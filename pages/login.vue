<template>
  <div class="vh-100 bg-default position-relative d-flex justify-content-center align-items-center">
    <div class="top-header h-50 bg-gradient-success position-absolute">
      <div class="separator separator-bottom separator-skew zindex-100">
        <svg x="0" y="0" viewBox="0 0 2560 100" preserveAspectRatio="none" version="1.1" xmlns="http://www.w3.org/2000/svg">
          <polygon points="2560 0 2560 100 0 100" class="fill-default"></polygon>
        </svg>
      </div>
    </div>
    <div class="col-lg-4 col-md-7">
      <div class="card bg-secondary shadow border-0">
        <div class="card-header bg-transparent">
          <div class="text-muted text-center mt-3 mb-3">
            <h2>💻 Point of Sale - Login</h2>
          </div>
          <div class="card-body px-lg-5 py-lg-3">
            <form role="form">
              <base-input 
                class="input-group-alternative mb-3"
                placeholder="Email"
                addon-left-icon="ni ni-email-83"
                v-model="model.email">
              </base-input>

              <base-input 
                class="input-group-alternative"
                placeholder="Password"
                type="password"
                addon-left-icon="ni ni-lock-circle-open"
                v-model="model.password">
              </base-input>
              <hr>
              <base-button block type="primary" class="my-4">Sign in</base-button>
            </form>
          </div>
        </div>
      </div>
      <div class="row mt-3">
        <div class="col-6">
          <a href="#" class="text-light">
            <small>Forgot Password?</small>
          </a>
        </div>
        <div class="col-6 text-right">
          <a href="#" class="text-light">
            <small>Create new account</small>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'login',
  data() {
    return {
      model: {
        email: '',
        password: ''
      }
    }
  }
}
</script>

<style scoped>
.top-header {
  top: 0;
  left: 0;
  right: 0;
}

.inside {
  bottom: 0;
}
</style>
