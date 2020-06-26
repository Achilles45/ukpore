<template>
  <div class="footer">
      <div class="container">
          <div class="row wrapper">
              <div class="col-md-3">
                  <h4>PHONE OR WHATSAPP</h4>
                  <p>+2349033369339</p>
                  <h6>Monday - Friday:</h6>
                  <p>Between 9am to 5pm WAT</p>
              </div>
                <div class="col-md-2">
                  <h4>QUICK LINKS</h4>
                  <ul>
                      <li><router-link to="/">Home</router-link></li>
                      <li><router-link to="/">About Us</router-link></li>
                      <li><router-link to="/">My Account</router-link></li>
                      <li><router-link to="/">Create An Account</router-link></li>
                  </ul>
              </div>
              <div class="col-md-4">
                  <h4>BANK PAYMENT DETAILS</h4>
                  <h6>Account Name: Africa Development Crowdfund Limited.</h6>
                  <h6>Account Number: 1016282563.</h6>
                  <h6>Bank: Zenith Bank Plc.</h6>
              </div>
              <div class="col-md-3">
                  <h4>OFFICE ADDRESS</h4>
                  <p>Royal Building (4th floor),
                    Lekki-Epe Expressway.
                    Ajiwe-Ajah
                    Opposite Fidelity Bank,
                    Lekki, Lagos State. Nigeria.</p>
              </div>
          </div>
      </div>
       <div class="footer__bottom">
          <div class="container">
              <div class="row">
                  <div class="col-md-4"></div>
                  <div class="col-md-4">
                      <small>Copylright &copy; 2020 <span class="wrap">African Development Crowdfund Limited | <a href="">Privacy Policy</a> | <a href="">Terms and Conditions</a></span></small>
                  </div>
                  <div class="col-md-4"></div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/styles/_colors';
.footer{
    background: $secondary-color;
    color: #fff;
    position: relative;
    // padding: 4rem 0;
    .wrapper{
        padding: 4rem 0;
        position: relative;
        h4{
            font-weight: 900;
            color: $tertiary-color;
            font-size: 1.3rem;
            padding-bottom: 1rem;
        }
        h6{
            line-height: 2;
        }
        ul{
            list-style: disc !important;
            li a{
                color: #fff;
                text-decoration: none;
            }
        }
    }
    .footer__bottom{
        background: $primary-color;
        padding-top: .8rem;
        padding-bottom: 1rem 3rem;
        a{
            color:#fff;
        }
        .wrap{
            opacity: .7;
        }
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    ul{
        padding-left: 2rem;
    }
    .footer__bottom{
        text-align: center;
        padding: 1rem 20 !important;
        a{
            color:#fff;
        }
    }
}
</style>
