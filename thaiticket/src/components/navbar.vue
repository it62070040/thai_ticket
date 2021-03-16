<template>
<nav class="navbar navbar-expand-lg navbar-light">
        <a class="navbar-brand" href="">
            <img src="./boot.png" width="30" height="30" alt="">
        </a>

        <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button> -->

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item"  @click="href=''">
                    <a class="nav-link" href="">หน้าแรก</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="">คอนเสิร์ต</a>
                </li>

            </ul>
            <form class="form-inline my-2 my-lg-0">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="">
                            <span class="icon">
                                <i><img src="https://img.icons8.com/ios-glyphs/30/000000/search.png"
                                        style="width:25px;" /></i>
                            </span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="">
                            <span class="icon">
                                <i><img src="https://img.icons8.com/pastel-glyph/64/000000/fast-delivery--v1.png"
                                        style="width:25px;" /></i>
                            </span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="">
                            <span class="icon">
                                <i><img src="https://img.icons8.com/material-rounded/24/000000/appointment-reminders.png"
                                        style="width:25px;" /></i>
                            </span>
                        </a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" id="navbarDropdown" role="button"
                            data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            ข้อมูลส่วนตัว
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a class="dropdown-item" href="//localhost:8080/#/user">ข้อมูลส่วนตัว</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="">
                                <span class="icon">
                                    <i><img src="https://img.icons8.com/carbon-copy/100/000000/ticket.png"
                                            style="width:20px;" /></i>
                                </span>
                                <span>ตั๋วของฉัน</span>
                            </a>s
                            <a class="dropdown-item" href="">
                                <span class="icon">
                                    <i><img src="https://img.icons8.com/wired/64/000000/list.png"
                                            style="width:20px;" /></i>
                                </span>
                                <span>ประวัติการสั่งซื้อ</span>
                            </a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="">
                                <span class="icon">
                                    <i><img src="https://img.icons8.com/ios/24/000000/edit--v1.png"
                                            style="width:20px;" /></i>
                                </span>
                                <span>แก้ไขข้อมูลส่วนตัว</span>
                            </a>
                            <a class="dropdown-item" href="">
                                <span class="icon">
                                    <i><img src="https://img.icons8.com/ios/26/000000/lock--v1.png"
                                            style="width:20px;" /></i>
                                </span>
                                <span>เปลี่ยนรหัสผ่าน</span>
                            </a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="">ออกจากระบบ</a>
                        </div>
                    </li>
                </ul>
            </form>
        </div>
    </nav>
</template>
<script>
export default {

}
</script>