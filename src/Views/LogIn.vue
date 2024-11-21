<script>
import logo from "../assets/cobach-logo.png";
export default {
  data() {
    return {
      logo,
    };
  },
};
</script>

<template>
  <div class="d-flex justify-content-center align-items-center vh-100">
    <div class="card shadow" style="width: 400px">
      <img :src="logo" class="card-img-top p-3" alt="Logo de la institución" />
      <div class="card-body">
        <h5 class="card-title text-center fw-bold">Iniciar sesión</h5>
        <p class="text-center">Accede con tu CURP y matrícula para continuar</p>
        <div class="form-floating mb-3">
          <input
            type="text"
            class="form-control"
            id="floatingcurp"
            placeholder="CURP"
          />
          <label for="floatingcurp">CURP</label>
        </div>
        <div class="form-floating mb-3">
          <input
            type="password"
            class="form-control"
            id="floatingmatricula"
            placeholder="matricula"
          />
          <label for="floatingmatricula">Matrícula</label>
        </div>
        <div class="text-center">
            <button type="submit" class="btn btn-primary w-50">Ingresar</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.d-flex {
  background-color: #e0f2ff;
}

.card-img-top {
  width: 50%;
  margin: 0 auto;
  display: block;
}
</style>
