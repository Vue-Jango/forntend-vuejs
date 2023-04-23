<script > 
export default {
  data() {
    return {
      login: "",
      password:""
    };
  },
  methods:{
    handelLogin(){
      console.log({
        login:this.login,
        password:this.password
      })
    }
  }

};
</script>

<template>
  <main>

    <div class="middle-box text-center loginscreen animated fadeInDown">
        <div>
            <div >

                <h2 style="font-size: 60px; display:flex; flex-direction: row; width: 3000px;" class="logo-name">Vue   &   jango</h2>
                <img style="height: 50px; width: 50px;" src="https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg"/>
              <img style="height: 50px; width: 50px;"  src="https://www.opengis.ch/wp-content/uploads/2020/04/django-python-logo.png"/>
            </div>
            <h3>Welcome Vue & jango</h3>
            <p> 
                this application is uses Vue Jango back end and implement JWT 
                see the base code on link 
                <!--Continually expanded and constantly improved Inspinia Admin Them (IN+)-->
            </p>
            <p>Login in. To see it in action.</p>
            <form class="m-t" role="form" action="http://webapplayers.com/inspinia_admin-v2.9.4/index.html">
                <div class="form-group">
                    <input type="email" v-model="login" class="form-control" placeholder="Username" required="">
                   <p style="color: red;"> {{ login }}</p>
                </div>
                <div class="form-group">
                    <input type="password"  v-model="password" class="form-control" placeholder="Password" required="">
                    <p style="color: red;"> {{ password }}</p>
                </div>
                <button type="button"  @click="handelLogin" class="btn btn-primary block full-width m-b">Login</button>

                <a href="#"><small>Forgot password?</small></a>
                <p class="text-muted text-center"><small>Do not have an account?</small></p>
                <a class="btn btn-sm btn-white btn-block" href="register.html">Create an account</a>
            </form>
            <p class="m-t"> <small>Inspinia we app framework base on Bootstrap 3 &copy; 2014</small> </p>
        </div>
    </div>

  </main>
</template>
