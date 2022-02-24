<template>
  <div class="MuayeneCell">

      <div class="row d-flex justify-content-around cell no-gutters ">
          <div class="col-12 col-lg-6 col-xl-4 colContainer firstBox">
 <div class="boxes">
          <div class="boxTitle redTitle">20 OCAK 2021 - 12:30</div>
          <div class="boxPara">Ataşehir Tıp Merkezi</div>
        </div> 
 <div class="col-12 col-lg-6 col-xl-4 colContainer doktorContainer">
    <div class="boxContainer">
          <img src="../../assets/anasayfa/doktor.svg" alt="" class="doktor" />
          <!-- flex column -->
          <div class="boxes">
            <div class="boxTitle">Prof. Dr. Mehmet Ali Tahaoğlu</div>
            <div class="boxPara">Gögüs Hastalıkları</div>
          </div>
        </div> 
          </div>
 <div class="col-12 col-lg-6 col-xl-4 colContainer ">
   <div class="boxContainer">
          <div class="icons">
            <div class="iconGroup">
              <img src="../../assets/anasayfa/lab.svg" alt="" class="icon" />
              <div class="iconPara">Lab</div>
            </div>
            <div class="iconGroup">
              <img
                src="../../assets/anasayfa/radyoloji.svg"
                alt=""
                class="icon"
              />
              <div class="iconPara">Radyoloji</div>
            </div>
            <div class="iconGroup">
              <img
                src="../../assets/anasayfa/patoloji.svg"
                alt=""
                class="icon"
              />
              <div class="iconPara">Patoloji</div>
            </div>
            <div class="iconGroup">
              <img src="../../assets/anasayfa/recete.svg" alt="" class="icon" />
              <div class="iconPara">Reçete</div>
            </div>
          </div>
        </div> 
      <div class="greyLine"></div>

      </div>



      </div>

      <div class="row bottomPart">
<div class="col-12 col-md-6 bottomPara d-flex justify-content-start">
<div class="row bottomParaRow">
    <div class="col-12 col-md-6 col-lg-6 paraItemContainer">
 <div class="paraItem">
                <img
                  src="../../assets/anasayfa/star.svg"
                  alt=""
                  class="paraIcon icon"
                />
                <div class="paraItemText">Puan Ver</div>
              </div>


    </div>


</div>

<div class="col-12 col-md-6 bottomButton d-flex justify-content-end">
<button class="btn">
            <p class="buttonPara">Randevu Alın</p>
          </button>

</div>

</div>




      </div>

    
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.MuayeneCell {
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
.greyLine {
  height: 1px;
  width: 95%;
  background: #dae9f1;
  margin-top: 20px;
  margin-bottom: 15px;
}
.cell {
  padding: 1rem;
  min-height: 180px;
  display: flex;
}
.colContainer {
  height: 100px;
  height: auto;
  padding: 0;
  margin: 0;
}
/* the following 2 are not visible. Kept them so that the layout wouldn't shift */
.logoBox {
  width: 40px;
  height: 170px;
  background: #fff9f0;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin-right: 20px;
  align-self: center;
  margin-left: 5px;
  opacity: 0;
}
.logo {
  height: 20px;
  width: 20px;
  /* margin-left: 1rem; */
  border-radius: 0px;
  margin: 0;
}
.boxes {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
.firstBox {
  padding-left: 20px;
}
.doktorContainer {
  padding-left: 1rem;
}
.boxTitle {
  width: auto;
  height: auto;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */
}
.greyTitle {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Primary */

  color: #3c4e69;
}
.boxPara {
  width: auto;
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
.redTitle {
  /* Kırmızı */
  color: #ea5455;
}
.boxContainer {
  display: flex;
  width: auto;
  justify-content: flex-end;
  align-items: center;
  min-height: auto;
  height: 100%;
  padding: 0;
  margin-bottom: 2rem;
}
.doktor {
  width: 50px;
  height: 50px;
  margin-right: 1rem;
}
.greyBox {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f2f8fb;
  border-radius: 5px;
  margin-right: 15px;
  /* this padding makes sure that the logo fits well */
  padding: 10px;
}
.greyLogo {
  width: 22px;
  height: 22px;
  margin-right: 1rem;
}
.bottomPara {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;
  /* Gri */

  color: #818b9a;
  padding: 0;
}
.bottomPart {
  padding: 0;
  margin: 0;
}
.bottomButton {
  /* border: solid; */
  padding: 0;
  padding-right: 1.4rem;
}
.btn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 250px;
  height: 40px;

  /* Button Primary */

  background: #ff7c32;
  border-radius: 6px;
}
.buttonPara {
  /* buton-text-kucuk */
  width: auto;
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
.icons {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-self: center;
}
.iconGroup {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-self: center;
  width: auto;
  height: auto;
}
.icon {
  width: auto;
  height: 18px;
  /* Primary */
  margin-bottom: 8px;
}
.iconPara {
  width: auto;
  height: auto;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */

  text-align: center;
  letter-spacing: -0.01em;

  /* Primary */

  color: #3c4e69;
}
.bottomParaRow {
  padding: 0;
  margin: 0;
  padding-left: 2.5rem;
}
.paraItemContainer {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-self: center;
  height: auto;
  padding: 0;
  margin: 0;
  margin-bottom: 1rem;
}
.paraItem {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-self: center;
  width: auto;
  height: auto;
}
.paraIcon {
  width: 22px;
  height: 22px;
  margin-right: 8px;
}
.paraItemText {
  width: auto;
  height: 21px;
  /* text3 */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */
  letter-spacing: -0.01em;
  /* Gri */
  color: #818b9a;
}

@media (max-width: 1200px) {
  .MuayeneCell {
    flex-direction: column;
  }

  .boxContainer {
    align-items: center;
  }
  .boxes {
    /* align-items: center; */
  }
  .logoBox {
    width: 100%;
    height: auto;
    padding: 10px;
    margin: 0;
  }
  .bottomParaRow {
    padding-left: 2rem;
  }
}
@media (max-width: 1000px) {
  .colContainer {
    margin-left: 1rem;
  }
}

@media (min-width: 1400px) {
  /* .bottomButton {
    padding-right: 3rem;
  } */
}
@media (max-width: 780px) {
  .bottomButton {
    padding: 0;
    /* this one makes the button look like as if it was centered in the cell */
    padding-left: 1.3rem;
  }
  .paraItemContainer {
    justify-content: center;
  }
  .btn {
    width: 100%;
  }
}
</style>
