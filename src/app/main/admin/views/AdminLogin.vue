<template>
    <div class="adminLogin">
        <header-slot>
            <div class="container-fluid">
                <h1 style="color:#fff">SayYesNo</h1>
            </div>
        </header-slot>
        <div class="adminLoginBlock">
            
                <div
          class="d-flex justify-content-center align-items-center adminLoginForm"
        >
          <div class="col col-sm-6 col-md-5 col-lg-4">
              <h2 class="text-center">Admin Login</h2>
            <form>
              <div class="mb-3">
                <label for="inputUserName" class="form-label">Username</label>
                <input
                  type="email"
                  class="form-control"
                  id="inputUserName"
                  aria-describedby="userName"
                />
              </div>
              <div class="mb-3">
                <label for="inputPassword" class="form-label">Password</label>
                <input
                  type="password"
                  class="form-control"
                  id="inputPassword"
                />
              </div>
            <div class="d-flex">
                 
                <div class="d-flex  flex-grow-1">
                    <a href="#">Froget Password</a>
                </div>
            </div>
              <div class="d-flex gap-4 justify-content-center">
             <a href="#" class="solidBtn">Login</a>
               

              </div>

             
            </form>
          </div>
        </div>
            
        </div>
    </div>
</template>

<script>
import HeaderSlot from '../../../slots/HeaderSlot.vue'
export default {
  components: { HeaderSlot },
    
}
</script>

<style scoped>
.adminLoginForm{
   height: calc(100vh - 80px);
    background: url(/img/loginFormbg.bd7b6105.png) center center;
    background-size: cover;
}
.adminLoginForm > div {
  background: rgb(225,216,227);
    background: linear-gradient(0deg, rgba(225,216,227,1) 0%, rgba(184,182,211,1) 100%);
    padding: 35px;
    border-radius: 7px;
}
.adminLoginForm:before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: var(--primary-color); 
    z-index: -1;
}
</style>