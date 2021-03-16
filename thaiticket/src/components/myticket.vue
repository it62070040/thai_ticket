<template>
  <div class="col-9">
    <div class="p-5" v-show="store.state.col1">
      <h3>ตั๋วของฉัน</h3>
    </div>

    <div class="p-5" v-show="store.state.col2">
      <h3>ประวัติการสั่งซื้อ</h3>
      <span style="font-weith: bold">งานแสดง</span>
    </div>
    <div class="p-5" v-show="store.state.col3">
      <h3>แก้ไขข้อมูลส่วนตัว</h3>
      <form >
        <div class="form-group">
          <label>ชื่อ</label>
          <input type="text" class="form-control" placeholder="ชื่อ" />
        </div>
        <div class="form-group">
          <label>นามสกุล</label>
          <input type="text" class="form-control" placeholder="นามสกุล" />
        </div>
        
        <select class="form-control">
          <option>ชาย</option>
          <option>หญิง</option>
          <option>อื่น</option>
        </select>

        <div class="form-control">
                <input type="date">
        </div>
        <div class="form-control">
                <input type="radio">
                <label for="">หมายเลขบัตรประชาชน</label>
                <input type="radio">
                <label for="">เลขที่หนังสือเดินทาง</label>
        </div>
        <div class="form-control">
                <input type="number">
                <label for="">หมายเลขโทรศัพท์</label>
        </div>

        <div class="form-control">
                <input type="text">
                <label for="">ที่อยู่</label>
        </div>
        <div class="form-control">
                <input type="text">
                <label for="">ประเทศ</label>
        </div>
        <div class="form-control">
                <select name="province">
      <option value="" selected>--------- เลือกจังหวัด ---------</option>
      <option value="กรุงเทพมหานคร">กรุงเทพมหานคร</option>
      <option value="กระบี่">กระบี่ </option>
      <option value="กาญจนบุรี">กาญจนบุรี </option>
      <option value="กาฬสินธุ์">กาฬสินธุ์ </option>
      <option value="กำแพงเพชร">กำแพงเพชร </option>
      <option value="ขอนแก่น">ขอนแก่น</option>
      <option value="จันทบุรี">จันทบุรี</option>
      <option value="ฉะเชิงเทรา">ฉะเชิงเทรา </option>
      <option value="ชัยนาท">ชัยนาท </option>
      <option value="ชัยภูมิ">ชัยภูมิ </option>
      <option value="ชุมพร">ชุมพร </option>
      <option value="ชลบุรี">ชลบุรี </option>
      <option value="เชียงใหม่">เชียงใหม่ </option>
      <option value="เชียงราย">เชียงราย </option>
      <option value="ตรัง">ตรัง </option>
      <option value="ตราด">ตราด </option>
      <option value="ตาก">ตาก </option>
      <option value="นครนายก">นครนายก </option>
      <option value="นครปฐม">นครปฐม </option>
      <option value="นครพนม">นครพนม </option>
      <option value="นครราชสีมา">นครราชสีมา </option>
      <option value="นครศรีธรรมราช">นครศรีธรรมราช </option>
      <option value="นครสวรรค์">นครสวรรค์ </option>
      <option value="นราธิวาส">นราธิวาส </option>
      <option value="น่าน">น่าน </option>
      <option value="นนทบุรี">นนทบุรี </option>
      <option value="บึงกาฬ">บึงกาฬ</option>
      <option value="บุรีรัมย์">บุรีรัมย์</option>
      <option value="ประจวบคีรีขันธ์">ประจวบคีรีขันธ์ </option>
      <option value="ปทุมธานี">ปทุมธานี </option>
      <option value="ปราจีนบุรี">ปราจีนบุรี </option>
      <option value="ปัตตานี">ปัตตานี </option>
      <option value="พะเยา">พะเยา </option>
      <option value="พระนครศรีอยุธยา">พระนครศรีอยุธยา </option>
      <option value="พังงา">พังงา </option>
      <option value="พิจิตร">พิจิตร </option>
      <option value="พิษณุโลก">พิษณุโลก </option>
      <option value="เพชรบุรี">เพชรบุรี </option>
      <option value="เพชรบูรณ์">เพชรบูรณ์ </option>
      <option value="แพร่">แพร่ </option>
      <option value="พัทลุง">พัทลุง </option>
      <option value="ภูเก็ต">ภูเก็ต </option>
      <option value="มหาสารคาม">มหาสารคาม </option>
      <option value="มุกดาหาร">มุกดาหาร </option>
      <option value="แม่ฮ่องสอน">แม่ฮ่องสอน </option>
      <option value="ยโสธร">ยโสธร </option>
      <option value="ยะลา">ยะลา </option>
      <option value="ร้อยเอ็ด">ร้อยเอ็ด </option>
      <option value="ระนอง">ระนอง </option>
      <option value="ระยอง">ระยอง </option>
      <option value="ราชบุรี">ราชบุรี</option>
      <option value="ลพบุรี">ลพบุรี </option>
      <option value="ลำปาง">ลำปาง </option>
      <option value="ลำพูน">ลำพูน </option>
      <option value="เลย">เลย </option>
      <option value="ศรีสะเกษ">ศรีสะเกษ</option>
      <option value="สกลนคร">สกลนคร</option>
      <option value="สงขลา">สงขลา </option>
      <option value="สมุทรสาคร">สมุทรสาคร </option>
      <option value="สมุทรปราการ">สมุทรปราการ </option>
      <option value="สมุทรสงคราม">สมุทรสงคราม </option>
      <option value="สระแก้ว">สระแก้ว </option>
      <option value="สระบุรี">สระบุรี </option>
      <option value="สิงห์บุรี">สิงห์บุรี </option>
      <option value="สุโขทัย">สุโขทัย </option>
      <option value="สุพรรณบุรี">สุพรรณบุรี </option>
      <option value="สุราษฎร์ธานี">สุราษฎร์ธานี </option>
      <option value="สุรินทร์">สุรินทร์ </option>
      <option value="สตูล">สตูล </option>
      <option value="หนองคาย">หนองคาย </option>
      <option value="หนองบัวลำภู">หนองบัวลำภู </option>
      <option value="อำนาจเจริญ">อำนาจเจริญ </option>
      <option value="อุดรธานี">อุดรธานี </option>
      <option value="อุตรดิตถ์">อุตรดิตถ์ </option>
      <option value="อุทัยธานี">อุทัยธานี </option>
      <option value="อุบลราชธานี">อุบลราชธานี</option>
      <option value="อ่างทอง">อ่างทอง </option>
      <option value="อื่นๆ">อื่นๆ</option>
                </select>
        </div>
        <div class="form-group">
          <label>อำเภอ</label>
          <input type="text"/>
        </div>
        <div class="form-group">
          <label>รหัสไปรษณีย์</label>
          <input type="number"/>
        </div>
        <button type="submit" class="btn btn-primary mb-2">บันทึก</button>
      </form>
    </div>
    <div class="p-5" v-show="store.state.col4">
        <h3>เปลี่ยนรหัสผ่าน</h3>
        <form>
        <div class="form-group">
          <label>รหัสผ่านเก่า</label>
          <input type="password" class="form-control" placeholder="ชื่อ" />
        </div>
        <span>รหัสผ่านใหม่(ต้องมีความยาว 8-16)</span>
        <div class="form-group">
          <label>รหัสผ่านใหม่</label>
          <input type="password" class="form-control" placeholder="นามสกุล" />
        </div>
        <div class="form-group">
          <label>ยืนยันรหัสผ่านใหม่</label>
          <input type="password" class="form-control" placeholder="นามสกุล" />
        </div>
        <button type="password" class="btn btn-primary mb-2">ตกลง</button>
        </form>
    </div>
  </div> 
</template>
<script>
import store from "@/vuex/store.js"
export default {
  data() {
    return {
      store
    }
  },
  methods: {
    
  },
  name: 'myticket',
}
</script>