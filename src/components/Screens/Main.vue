<template>
  <div class="edit-form container">
    <div class="row">
      <div class="col-sm col-md col-lg-5 shadow3" style="cursor: pointer;" onclick="window.location='/customer';">
        <h4 class="differ3">Cliente</h4>
      </div>
      <div class="col-sm-6 col-md-6 col-lg-5 shadow2" style="cursor: pointer;" onclick="window.location='/owner';">
        <h4 class="differ2">Empresa</h4>
      </div>
    </div>
  </div>
</template>
<script>
</script>

<style scoped>

.shadow3 {
  z-index: 10;
  height: 100px;
  border: 1px white;
  box-shadow: 0 0 0 3px #ffffff;
  margin-top: 180px;
  margin-left: 1020px;
  padding: 10px;
}
.differ3{
    margin-left: 155px;
    margin-top: 20px;
    letter-spacing: 5px;
  font-family: Raleway;
  font-weight: bolder;
  font-size: 40px;
  color: #ffffff;
}
.shadow2 {
  z-index: 10;
  height: 100px;
  border: 1px white;
  box-shadow: 0 0 0 3px #ffffff;
  margin-top: 60px;
  margin-left: 1020px;
  padding: 10px;
}
.differ2{
  margin-left: 150px;
  margin-top: 20px;
  letter-spacing: 5px;
  font-family: Raleway;
  font-size: 40px;
  font-weight: bolder;
  color: #ffffff;
}

</style>
