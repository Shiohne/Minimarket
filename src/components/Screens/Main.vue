<template>
  <div class="edit-form container">
    <div class="row">
      <div class="col-sm col-md col-lg-5 shadow" style="cursor: pointer;" onclick="window.location='/customer';">
        <h4 class="differ">CLIENTE</h4>
      </div>
      <div class="col-sm-6 col-md-6 col-lg-5 shadow" style="cursor: pointer;" onclick="window.location='/owner';">
        <h4 class="differ">EMPRESA</h4>
      </div>
    </div>
  </div>
</template>
<script>
</script>

<style scoped>

.shadow {
  z-index: 10;
  height: 100px;
  background: #f38701;
  margin-top: 120px;
  margin-left: 1020px;
  border-width: 100px;
  padding: 10px;
}
.differ{
    margin-left: 180px;
    margin-top: 20px;
    letter-spacing: 5px;
  font-family: Roboto;
  font-weight: bolder;
  color: #ffffff;
}

</style>
