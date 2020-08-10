<template>
  <div>
    <div class="modal">
      <img src="../assets/S__33177618.jpg" alt="" />
      <div class="close"></div>
    </div>
    <div class="container">
      <div class="card">
        <div class="header">
          <div class="hamburger-menu">
            <div class="center"></div>
          </div>
          <a href="#" class="mail">
            <i class="far fa-envelope"></i>
          </a>
          <div class="main">
            <div class="image">
              <div class="hover">
                <i class="fas fa-camera fa-2x"></i>
              </div>
            </div>
            <h3 class="name">Cheer Dyw</h3>
            <h3 class="sub_name">@cheerdyw</h3>
          </div>
        </div>
        <div class="content">
          <div class="left">
            <div class="about-container">
              <h3 class="title">About</h3>
              <p class="text">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry.
              </p>
            </div>
            <div class="icons-container">
              <a href="#" class="icon">
                <i class="fab fa-facebook"></i>
              </a>
              <a href="#" class="icon">
                <i class="fab fa-instagram"></i>
              </a>
              <a href="#" class="icon">
                <i class="fab fa-google-plus-g"></i>
              </a>
              <a href="#" class="icon">
                <i class="fab fa-twitter"></i>
              </a>
            </div>
            <div class="buttons-wrap">
              <div class="follow-wrap">
                <a href="" class="follow">Follow</a>
              </div>
              <div class="share-wrap">
                <a href="" class="share">Share</a>
              </div>
            </div>
          </div>
          <div class="right">
            <div>
              <h3 class="number">91</h3>
              <h3 class="number-title">Posts</h3>
            </div>
            <div>
              <h3 class="number">2.4K</h3>
              <h3 class="number-title">Following</h3>
            </div>
            <div>
              <h3 class="number">4.7K</h3>
              <h3 class="number-title">Followers</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}
body {
  background-color: #efefef;
}
.container {
  padding: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
.card {
  position: relative;
  width: 400px;
  background-color: #fff;
  border-radius: 5px;
  box-shadow: 0 5px 15px 1px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}
.card:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 270px;
  top: 0;
  left: 0;
  background-image: linear-gradient(to top, #00f2fe, #4facfe);
  clip-path: circle(400px at 50% -48.5%);
}
.header {
  position: relative;
  height: 265px;
}
.mail {
  position: absolute;
  top: 1rem;
  right: 2rem;
  font-size: 1.5rem;
  color: #fff;
  opacity: 0.8;
  transition: 0.3s;
  z-index: 3;
}
.mail:hover {
  opacity: 1;
}
.hamburger-menu {
  position: absolute;
  width: 21px;
  height: 16px;
  top: 1.4rem;
  left: 1.9rem;
  z-index: 3;
  cursor: pointer;
  opacity: 0.8;
  transition: 0.3s;
}
.hamburger-menu:hover {
  opacity: 1;
}
.hamburger-menu .center {
  position: absolute;
  height: 2px;
  width: 70%;
  top: 50%;
  transform: translateY(-50%);
  background-color: #fff;
  border-radius: 1px;
}

.hamburger-menu:before,
.hamburger-menu:after {
  content: "";
  position: absolute;
  width: 100%;
  right: 0;
  height: 2px;
  border-radius: 1px;
  background-color: #fff;
}
.hamburger-menu:before {
  top: 0;
}
.hamburger-menu:after {
  bottom: 0;
}
.main {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.main .image {
  position: relative;
  width: 110px;
  height: 110px;
  border-radius: 50%;
  background: url("../assets/S__33177618.jpg") no-repeat center / cover;
  border: 4px solid #00d8fe;
  margin-bottom: 2px;
  overflow: hidden;
  cursor: pointer;
}
.image .hover {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background: rgba(79, 172, 254, 0.7);
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  transition: 0.5s;
  opacity: 0;
}

.image:hover .hover {
  opacity: 1;
}

.name {
  font-size: 1.2rem;
  color: #fff;
  font-weight: 500;
  line-height: 1;
  margin: 5px 0;
}
.sub_name {
  font-family: "Cutive Mono", monospace;
  font-size: 1.2rem;
  opacity: 0.8;
  color: #fff;
}
.content {
  display: flex;
  padding: 1.7rem 2.5rem 2.6rem 2.5rem;
}

.right {
  padding-top: 1.5rem;
  display: flex;
  flex-direction: column;
  text-align: right;
  align-items: flex-end;
  justify-content: space-between;
  margin-left: 2.1rem;
}
.number {
  font-size: 2.1rem;
  font-weight: 200;
  color: #333;
  line-height: 1.2;
}
.number-title {
  font-size: 0.55rem;
  font-weight: 400;
  color: #666;
  line-height: 1;
  letter-spacing: 1px;
  text-transform: uppercase;
}
.left {
  display: flex;
  flex-direction: column;
  text-align: left;
}
.title {
  position: relative;
  font-size: 1.1rem;
  font-weight: 500;
  color: #555;
  padding: 0 0 3px 0;
  margin-bottom: 0.9rem;
  display: inline-block;
}
.title::after {
  content: "";
  position: absolute;
  height: 3px;
  width: 50%;
  background-color: #555;
  bottom: 0;
  left: 0;
}
.text {
  font-weight: 300;
  color: #666;
  line-height: 1.7;
}
.icons-container {
  padding: 1rem 0;
}
.icon {
  color: #c4c4c4;
  font-size: 1.3rem;
  text-decoration: none;
  margin-right: 8px;
  transition: 0.3s;
}
.icon:hover {
  color: #4facfe;
}
.buttons-wrap {
  display: flex;
  margin-top: 5px;
}
.follow-wrap,
.share-wrap {
  flex: 4;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.5s;
}
.follow-wrap:hover,
.share-wrap:hover {
  flex: 5;
}

.follow {
  padding: 9.6px 0;
  width: 100%;
  background: linear-gradient(to right, #4facfe 0%, #00f2fe 140%);
  color: #fff;
  text-align: center;
  text-decoration: none;
  font-size: 0.7rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  border-radius: 18.1px;
  margin-right: 3px;
}
.share {
  padding: 7.6px 0;
  width: 100%;
  border: 2px solid #4facfe;
  color: #4facfe;
  text-decoration: none;
  text-align: center;
  font-size: 0.7rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  margin-left: 3px;
  border-radius: 18.1px;
}
.modal {
  position: fixed;
  width: 100%;
  height: 100vh;
  background: rgba(0, 0, 0, 0.8);
  z-index: -1;
  opacity: 0;
  transition: .5s;
}
.modal img {
  position: absolute;
  top: 25%;
  left: 50%;
  transform: translate(-50%, -50%) scale(.3);
  max-width: 100%;
  max-height: 100%;
  transition: .5s;
}
.modal.show{
  opacity: 1;
  z-index: 99;
}
.modal.show img{
  top: 50%;
  transform: translate(-50%, -50%) scale(1);
}
.close {
  position: absolute;
  top: 1rem;
  right: 1rem;
  width: 30px;
  height: 30px;
  cursor: pointer;
  transition: .3s;
}
.close:hover {
  opacity: .5;
}
.close:before, .close:after {
  content: "";
  position: absolute;
  width: 100%;
  height: 3px;
  border-radius: 1.5px;
  top: 50%;
  right: 50%;
  background-color: #fff;
}
.close:before{
  transform: translate(-50%, -50%) rotate(45deg);
}
.close:after{
  transform: translate(-50%, -50%) rotate(135deg);
}
</style>
