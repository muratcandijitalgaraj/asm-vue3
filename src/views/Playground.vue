<template>
  <div class="playground">{{ info }}</div>
  <!-- Button trigger modal -->
  <button
    type="button"
    class="btn btn-primary clicky"
    data-bs-toggle="modal"
    data-bs-target="#staticBackdrop"
  >
    Launch static backdrop modal
  </button>

  <!-- Modal 
  shall add this later on
    data-bs-backdrop="static"-->
  <div
    class="modal fade"
    id="staticBackdrop"
    data-bs-keyboard="false"
    tabindex="-1"
    aria-labelledby="staticBackdropLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-body modalItemsContainer">
          <!-- <img src="" alt="" class="modalImage"> -->
          <div class="modalTitle">Bu Kullanıcı hesabı size mi ait?</div>
          <div class="modalText">
            Girmiş olduğunuz 0555 666 77 88 telefon numarası A** Y***** adına
            kayıtlıdır
          </div>
          <button class="positiveBtn">
            <div class="modalButtonText" data-bs-dismiss="modal">
              Evet, bu hesap bana ait
            </div>
          </button>
          <button class="negativeBtn">
            <div class="modalButtonText">Hayır, hesap bana ait değil</div>
          </button>
        </div>
        <div class="modal-footer"></div>
      </div>
    </div>
  </div>
</template>

<script>
// axios.<method> will now provide autocomplete and parameter typings
import axios from "axios";
//this library ensures that url encoded headers are read correctly.
//Without it the logic doesn't work
import qs from "qs";
export default {
  data() {
    return {
      info: null,
    };
  },
  async mounted() {
    try {
      const url = "http://localhost:8080/connect/token";
      const data = {
        client_id: "iCoMed_Mobile_IOS",
        client_secret: "c@mEd3234_21!",
        grant_type: "client_credentials",
      };
      const options = {
        method: "POST",
        headers: { "content-type": "application/x-www-form-urlencoded" },
        data: qs.stringify(data),
        url,
      };
      let res = await axios(options);
      console.log(res.data);
    } catch (err) {
      console.log(err);
    }
    document.querySelector(".clicky").click();
  },
};
</script>

<style>
.modal-content {
  width: 470px;
  height: 571px;

  background: #e9f3f9 !important;
  border-radius: 16px;
}
.clicky {
  display: none;
}
.modalItemsContainer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.modalTitle {
  width: 308px;
  height: 26px;

  /* baslik */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 20px;
  line-height: 130%;
  /* identical to box height, or 26px */

  text-align: center;
  letter-spacing: -0.01em;

  /* Primary */

  color: #3c4e69;
  margin-bottom: 14px;
}
.modalText {
  width: 295px;
  height: 42px;

  /* text02 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 140%;
  /* or 21px */

  text-align: center;

  /* Primary */

  color: #3c4e69;
  margin-bottom: 60px;
}
.positiveBtn,
.negativeBtn {
  width: 341px;
  height: 50px;
  border: none;
  border-radius: 6px;
  margin-bottom: 20px;
}
.positiveBtn {
  background: #ff7c32;
}
.negativeBtn {
  background: #2e95df;
}
.modalButtonText {
  /* buton-text */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 16px;
  line-height: 130%;
  /* identical to box height, or 21px */

  text-align: center;

  /* Beyaz */

  color: #ffffff;
}
</style>
