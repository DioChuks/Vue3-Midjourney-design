<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
    <div class="myBlurRight"></div>
  <div class="container" id="myCustomContainer">
    <header>
      <nav class="navbar navbar-expand-md navbar-dark">
        <div class="container-fluid" id="myContainerFluid">
          <RouterLink class="navbar-brand" to="/">
            <img
              src="../assets/pngtree-removebg-preview.png"
              class="d-inline-block"
            />
            Quintessence
          </RouterLink>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarNavDropdown"
            aria-controls="navbarNavDropdown"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav" id="nav" style="margin-left: auto;">
              <li class="nav-item">
                <RouterLink class="nav-link active" aria-current="page" to="/">Home</RouterLink>
              </li>
              <li class="nav-item">
                <RouterLink class="nav-link" to="/features">Features</RouterLink>
              </li>
              <li class="nav-item">
                <RouterLink class="nav-link" to="/pricing">Pricing</RouterLink>
              </li>
              <li class="nav-item dropdown" id="account">
                <a
                  class="nav-link dropdown-toggle"
                  href="#"
                  id="navbarDropdownMenuLink"
                  role="button"
                  data-bs-toggle="dropdown"
                  aria-expanded="false"
                >
                  Account
                </a>
                <ul
                  class="dropdown-menu"
                  aria-labelledby="navbarDropdownMenuLink"
                  id="dropdownMenu"
                >
                  <li><RouterLink class="dropdown-item" to="/login">Login</RouterLink></li>
                  <li><RouterLink class="dropdown-item" to="/signup">Sign-up</RouterLink></li>
                </ul>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </header>
  </div>
  <div class="myBlurBottom"></div>
</template>

<style lang="scss" scoped>
.myBlurRight{
    z-index: 1;
    width: auto;
    height: 100px;
    flex-shrink: 0;
    background: linear-gradient(90deg, rgba(0, 0, 0, 0.08) 0%, rgba(0, 0, 0, 0.00) 100%);
    filter: blur(12.5px);
    backdrop-filter: blur(12.5px);
}
.myCustomContainer{
    margin-top: -50px;
}
#myContainerFluid{
    margin-top: -100px;
}
#nav{
    border-radius: 10px;
    .nav-item{
        gap: 10px;
        margin-left: 30px;
    }
    #account{
        border-radius: 10px;
        filter: blur(.5px);
        background: linear-gradient(180deg, rgba(254, 200, 241, 0.90) 0%, rgba(237, 146, 215, 0.00) 40.39%), radial-gradient(96.63% 140.33% at 76.68% 66.67%, rgba(96, 46, 166, 0.00) 0%, rgba(201, 119, 214, 0.50) 100%);
        background-blend-mode: overlay, normal;
        box-shadow: 0px 10px 10px 0px rgba(0, 0, 0, 0.10), 0px 0px 5px 0px #FFACE4 inset, 0px -1px 8px 0px #9375B6 inset;
        #dropdownMenu{
            border-radius: 10px;
            background: linear-gradient(180deg, rgba(254, 200, 241, 0.90) 0%, rgba(237, 146, 215, 0.00) 40.39%), radial-gradient(96.63% 140.33% at 76.68% 66.67%, rgba(96, 46, 166, 0.00) 0%, rgba(201, 119, 214, 0.50) 100%);
            box-shadow: 0px 10px 10px 0px rgba(0, 0, 0, 0.10), 0px 0px 5px 0px #FFACE4 inset, 0px -1px 8px 0px #9375B6 inset;
        }
        #dropdownMenu li:hover{
            background: linear-gradient(180deg, rgba(254, 200, 241, 0.90) 0%, rgba(237, 146, 215, 0.00) 40.39%), radial-gradient(96.63% 140.33% at 76.68% 66.67%, rgba(96, 46, 166, 0.00) 0%, rgba(201, 119, 214, 0.50) 100%);
        }
        #dropdownMenu li a{
            color: #FFF;
            background: none;
        }
    }
}
.myBlurBottom{
    display: none;
    width: auto;
    height: 216.5px;
    flex-shrink: 0;
    background: linear-gradient(90deg, rgba(0, 0, 0, 0.10) 0%, rgba(0, 0, 0, 0.00) 100%);
    filter: blur(50px);
    backdrop-filter: blur(30px);
}
</style>
