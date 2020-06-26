<template>
  <div class="navbar__wrapper container-fluid">
      <div class="navbar__holder">
          <div class="navbar__content d-flex justify-content-between align-items-center">
              <div class="logo pt-2">
                  <router-link to="/" class="logo"><img src="../assets/images/logo.png" class="logo__img" alt=""></router-link>
              </div>
              <div class="menu">
                  <ul class="d-flex justify-content-between pt-3">
                      <li><router-link to="/" class="links">Home</router-link></li>
                      <li><router-link to="/" class="links">About Us</router-link></li>
                      <li><router-link to="/" class="links">My Account</router-link></li>
                      <li><router-link to="/" class="links create">Create an Account</router-link></li>
                  </ul>
              </div>
              <div @click="showNav()" class="navbar__toggler"> 
                    <div class="holder d-flex justify-content-between align-items-center">
                    <i class="fa fa-bars"></i>
                    <p class="pt-3 pl-2">Menu</p>
                    </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    methods:{
        //  logOut:function(){
        //    firebase.auth().signOut()
        //    .then(()=>{
        //        this.$router.push({name: 'Signin'})
        //    })
        // },
        showNav:function(){
            const navbarToggler = document.querySelector('.navbar__toggler');
            const nav = document.querySelector('.menu');
            const navLinks = document.querySelector('.links')
            nav.classList.toggle('show__nav');
            navLinks.classList.remove('show__nav');
        },
        fixNav:function(){
             const nav = document.querySelector('.navbar__wrapper');
            window.onscroll = function(){
                if (window.pageYOffset > 150) {
                    nav.classList.add('fix__nav');
                }else{
                    nav.classList.remove('fix__nav');
                }
            }
        },
 },
//  mounted(){
//      this.fixNav()
//  }
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/colors';
.navbar__wrapper{
    background: $primary-color;
    padding: .9rem 0;
    position: relative;
    .navbar__holder{
        padding: 0 2rem;
        margin: 0 auto;
    }
    .navbar__content{
        .logo{
             text-decoration: none !important;
            //  color: #fff;
            h4{
                color: $primary-color;
                font-weight: bolder;
                font-size: 1rem;
            }
            .logo__img{
                max-width: 320px;
                height: auto;
            }
        }
        .menu{
            ul li a{
                text-decoration: none;
                margin: 0 1rem;
                font-weight: bolder;
                // opacity: .8;
                color:#fff;
                text-transform: capitalize;
                font-size: 1rem;
            }
            .create{
                padding: .6rem 2rem;
                border-radius: 6px;
                background: $secondary-color;
                color: #fff;
                font-weight: normal !important;
                opacity: 1 !important;
            }
        }
        .navbar__toggler{
            display: none;
            font-size: 1.2rem;
            padding-right: 1rem;
            color: $secondary-color !important;
        }
    }
}
//Fix navigation
.fix__nav{
    position: fixed;
    top: 0; 
    width: 100%;
    z-index: 100;
    background: #fff;
    padding: .8rem 0;
    transition: all ease-in-out .5s;
    box-shadow: 0px 0px 5px rgba(0,0,0,0.17);
    a{
           color: $primary-color !important;
           opacity: .8 !important;
    }
    .login{
        color: #fff !important;
    }
}

//Show Navigation
.show__nav{
    display: block !important;
    transition: all ease-in .5s;
}
//MEDIA QUERIES
@media only screen and (max-width: 1100px){
    .navbar__wrapper{
        padding: 1rem 1rem !important;
    }
    .navbar__holder{
        padding: 0 1.2rem !important;
    }
    .logo__img{
        max-width: 200px !important;
        height: auto;
    }
    .fa-bars{
        color: $tertiary-color;
    }
    p{
        color: #fff;
    }
    .menu{
        background-color: $primary-color;
        width: 85%;
        position: absolute;
        height: auto !important;
        z-index: 100;
        height: 100vh -50% !important;
        display: none;
        border-top: 3px solid $tertiary-color;
        padding: 0 1rem !important;
        margin: 0 auto !important;
        transition: 0.5s !important;
        top: 100%;
        left: 7%;
        ul{
            flex-direction: column;
            li a{
                color: #fff !important;
                line-height: 4;
            }
            .create{
                background: #008E51 !important;
                color: #fff !important;
                width: 90% !important;
                display: inline-block !important;
                padding: 0rem 2rem !important;
                height: 3.5rem;
            }
        }
    }
    .navbar__toggler{
        display: block !important;
        color: #fff !important;
    }
}
</style>