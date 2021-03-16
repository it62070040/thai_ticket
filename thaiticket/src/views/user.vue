<template>
  <div class="container-fluid p-3">
    <div class="row">
      <div
        class="col-3 justify-content-center d-flex"
        style="border-color: gray;background-color: #E1E1E1;"
      >
        <div class="profile">
          <img
            src="./images/boot.png"
            alt=""
            class="m-5"
            style="border-radius: 100%; width: 3vw; text-align: center"
          />
          <div class="mb-5">
            <span>chanakan thudhayanukul</span>
            <span class="d-block">chanakan@gmail.com</span>
          </div>
          <div class="mb-5">
            <span class="icon d-block" @click="showTicket()">
              <i
                ><img
                  src="https://img.icons8.com/carbon-copy/100/000000/ticket.png"
                  style="width: 3vw" /></i
              >ตั๋วของฉัน
            </span>
            <span class="icon d-block" @click="showHistory()">
              <i
                ><img
                  src="https://img.icons8.com/wired/64/000000/list.png"
                  style="width: 20px" /></i
              >ประวัติการสั่งซื้อ
            </span>
            <hr />
            <span class="icon d-block" @click="showEditProfile()">
              <i
                ><img
                  src="https://img.icons8.com/ios/24/000000/edit--v1.png"
                  style="width: 20px" /></i
              >แก้ไขข้อมูลส่วนตัว
            </span>
            <span class="icon d-block" @click="showChangePassword()">
              <i
                ><img
                  src="https://img.icons8.com/ios/26/000000/lock--v1.png"
                  style="width: 20px" /></i
              >เปลี่ยนรหัสผ่าน
            </span>
            <hr />
            <a class="dropdown-item" href="#">ออกจากระบบ</a>
          </div>
        </div>
      </div>
      <myticket />
    </div>
  </div>
</template>
<script>
import myticket from "../components/myticket";
import store from "@/vuex/store.js";
export default {
  data() {
    return {
      store,
    };
  },
  components: {
    myticket,
  },
  methods: {
    showTicket() {
      this.store.state.col1 = true;
      this.store.state.col2 = false;
      this.store.state.col3 = false;
      this.store.state.col4 = false;
    },
    showHistory() {
      this.store.state.col1 = false;
      this.store.state.col2 = true;
      this.store.state.col3 = false;
      this.store.state.col4 = false;
    },
    showEditProfile() {
      this.store.state.col2 = false;
      this.store.state.col1 = false;
      this.store.state.col3 = true;
      this.store.state.col4 = false;
    },
    showChangePassword() {
      this.store.state.col2 = false;
      this.store.state.col1 = false;
      this.store.state.col3 = false;
      this.store.state.col4 = true;
    },
  },
};
</script>