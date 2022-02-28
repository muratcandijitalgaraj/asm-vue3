<template>
  <div class="randevularimTop">
    <div class="row">
      <div
        class="col randevularimContainer d-flex align-items-center justify-content-start"
      >
        <div class="randevularimText">Randevularım</div>
      </div>
      <div class="col">
        <div
          class="yerindeRandevular d-flex align-items-center justify-content-center"
        >
          Yerinde Randevular
        </div>
        <div class="selectedTab d-flex justify-content-end"></div>
      </div>
      <div class="col goruntulu d-flex align-items-center">
        Görüntülü Görüşme
      </div>
      <div class="col d-flex justify-content-end">
        <button class="button">
          <div class="buttonText">Yeni Randevu Alın</div>
        </button>
      </div>
    </div>
    <!-- row ends -->
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.col {
  /* display: flex;
  align-items: center; */
}
.randevularimTop {
  padding-top: 15px;
}
.randevularimContainer {
}
.randevularimText {
  width: 142px;
  height: auto;

  /* baslik3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */

  /* Primary */

  color: #3c4e69;
  margin-left: 1rem;
}
.yerindeRandevular {
  width: auto;
  height: 100%;
  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Secondary */

  color: #32a5df;
}
.goruntulu {
  width: 148px;

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
.button {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 167px;
  height: 40px;

  /* Button Primary */

  background: #ff7c32;
  border: none;
  border-radius: 6px;
}
.buttonText {
  width: 127px;
  height: 17px;

  /* buton-text-kucuk */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 110%;
  /* identical to box height, or 17px */

  display: flex;
  align-items: center;
  text-align: center;

  /* Beyaz */

  color: #ffffff;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;
}
</style>
