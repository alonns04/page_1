

<script>
export default {
  data() {
    return {
      selectedProvincia: 0,
      selectedMunicipio: 0,
      selectedLocalidad: 0,
      provincias: [],
      municipios: [],
      localidades: [],
    };
  },
  mounted() {
    this.fetchProvincias();
  },
  methods: {
    fetchProvincias() {
      fetch("https://apis.datos.gob.ar/georef/api/provincias")
        .then(res => res.ok ? res.json() : Promise.reject(res))
        .then(json => {
          this.provincias = json.provincias.sort((a, b) => a.nombre.localeCompare(b.nombre));
        });
    },
    municipio() {
      if (this.selectedProvincia !== 0) {
        fetch(`https://apis.datos.gob.ar/georef/api/municipios?provincia=${this.selectedProvincia}&max=135`)
          .then(res => res.ok ? res.json() : Promise.reject(res))
          .then(json => {
            this.municipios = json.municipios.sort((a, b) => a.nombre.localeCompare(b.nombre));
          });
      }
    },
    localidad() {
      if (this.selectedMunicipio !== 0) {
        fetch(`https://apis.datos.gob.ar/georef/api/localidades?municipio=${this.selectedMunicipio}&max=30`)
          .then(res => res.ok ? res.json() : Promise.reject(res))
          .then(json => {
            this.localidades = json.localidades.sort((a, b) => a.nombre.localeCompare(b.nombre));
          });
      }
    },
  },
};
</script>



<template>
  <div style="padding: 46px 0 10px 0;">
  <div class="container">
    <div class="row">
      <div class="form-group col-12">
        <label for="inputEmail4">Correo Electrónico</label>
        <input type="email" class="form-control" id="inputEmail4" placeholder="Email@ejemplo.com">
      </div>
      <div class="form-group col-12">
        <label for="inputAddress">Dirección</label>
        <input type="text" class="form-control" id="inputAddress" placeholder="0000, 9 de Julio">
      </div>
      <div class="col-12">
        <label>Provincia</label>
        <select class="form-control" v-model="selectedProvincia" @change="municipio">
          <option value="0">Seleccione su provincia</option>
          <option v-for="provincia in provincias" :key="provincia.id" :value="provincia.id">{{ provincia.nombre }}
          </option>
        </select>
      </div>
      <div class="col-6">
        <label>Municipio</label>
        <select class="form-control" v-model="selectedMunicipio" @change="localidad">
          <option value="0">Seleccione su municipio</option>
          <option v-for="municipio in municipios" :key="municipio.id" :value="municipio.id">{{ municipio.nombre }}
          </option>
        </select>
      </div>
      <div class="col-6">
        <label>Localidad</label>
        <select class="form-control" v-model="selectedLocalidad">
          <option value="0">Seleccione su localidad</option>
          <option v-for="localidad in localidades" :key="localidad.id" :value="localidad.id">{{ localidad.nombre }}
          </option>
        </select>
      </div>
      <div class="col-12 text-end mx-auto">
        <button style="margin-top: 10px;" type="submit" class="btn btn-light">Enviar</button>
      </div>
    </div>
  </div>
</div>
</template>


<style scoped>
div {
  background-color: black !important;
  color: white !important;
}
</style>