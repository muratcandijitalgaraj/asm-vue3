<template>
  <div class="cellComponent row">
    <div class="logoBox">
      <img src="../../assets/anasayfa/gorusme.svg" alt="" class="logo" />
    </div>
    <!-- first box -->
    <div
      class="col box 1stBox d-flex flex-column justify-content-center align-items-start"
    >
      <div class="row colTitle redTitle">Görüşme Bekleniyor</div>
      <div class="row colPara">20 Ocak Pazartesi - 12:30</div>
    </div>
    <div
      class="col box 1stBox d-flex flex-column justify-content-center align-items-start"
    >
      <div class="row colTitle redTitle">Görüşme Bekleniyor</div>
      <div class="row colPara">20 Ocak Pazartesi - 12:30</div>
    </div>
    <div
      class="col box 1stBox d-flex flex-column justify-content-center align-items-start"
    >
      <div class="row colTitle redTitle">Görüşme Bekleniyor</div>
      <div class="row colPara">20 Ocak Pazartesi - 12:30</div>
    </div>

    <!-- second box -->

    <!-- third box -->
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.cellComponent {
  display: flex;
  margin-left: 12px;
  background: #ffffff;
  /* Boxx Shadow */
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  margin-bottom: 20px;
  margin-top: 20px;
  height: auto;
}
.cell {
  width: auto;
  height: 100%;
}
.col {
  height: 100%;
}
.box {
  height: 100%;
}
.colTitle {
  width: 225px;
  height: 24px;
  /* baslik4 */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */
  /* Primary */
  color: #3c4e69;
}
.redTitle {
  color: #ea5455;
}
.colPara {
  width: 171px;
  height: 21px;
  /* text3 */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */
  letter-spacing: -0.01em;
  /* Primary */
  color: #3c4e69;
}
.logoBox {
  width: 40px;
  height: 100px;
  background: #ffeeee;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin-right: 20px;

  align-self: center;
  margin-left: 5px;
}
.logo {
  height: 20px;
  width: 20px;
  /* margin-left: 1rem; */
  border-radius: 0px;
  margin: 0;
}

@media (max-width: 1200px) {
  .cellComponent {
    flex-direction: column;
  }
  .logoBox {
    width: 100%;
    height: auto;
    padding: 10px;
    margin: 0;
  }
}
@media (max-width: 1000px) {
}
</style>
