<template>
  <div class="container-fluid">
    <div class="d-flex justify-content-around ">
      <b-navbar class="nav" toggleable="lg" type="dark" variant="transparent">
        <b-navbar-brand href="#">
          <img src="../assets/Logotype.png" class="LogoImage"
        /></b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav >
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto text_color">
            <b-nav-item-dropdown right >
              <!-- Using 'button-content' slot -->
              <template #button-content>
                <em >Demos</em>
              </template>
              <b-dropdown-item href="#">*</b-dropdown-item>
              <b-dropdown-item href="#">*</b-dropdown-item>
            </b-nav-item-dropdown>

            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template #button-content>
                <em>Pages</em>
              </template>
              <b-dropdown-item href="#">*</b-dropdown-item>
              <b-dropdown-item href="#">*</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template #button-content>
                <em>Features</em>
              </template>
              <b-dropdown-item href="#">*</b-dropdown-item>
              <b-dropdown-item href="#">*</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown>
              <template #button-content>
                <em>Tutorials</em>
              </template>
            </b-nav-item-dropdown>
            <div><b-button variant="warning">Purchase</b-button></div>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.navbar{
  width: 60%;
  color: white;
}
em {
  color: white;
}
.nav {
  z-index: 2;
  position: absolute;
}
.text_color > *{
  font-size: 18px;
  color: white;
}
@media only screen and (max-width: 650px) {
.LogoImage{
  width: 70%;
}
.nav {
  
  background-color: silver;
  z-index: 2;
  position: absolute;
}
.navbar{
  width: 100%;
}
}
</style>