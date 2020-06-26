<template>
  <div class="home">
    <Navbar />
    <div class="heading__wrapper">
      <div class="container">
        <div class="row">
          <div class="col-md-12 text-center">
            <h1>Invest Now</h1>
            <p>Your investment helps develop Africa and makes money work for you.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="intro__section">
     <div class="container">
        <div class="row">
        <div class="col-12 text1">
          <h5>Make payment to the account details below. When we confirm your payment, we will send to your email, a payment receipt and an MOU/Contract Agreement.</h5>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6 text2">
          <h4>BANK TRANSFER PAYMENT DETAILS</h4>
          <h5><strong>Account Name:</strong> Africa Development Crowdfund Limited.</h5>
          <h5><strong>Account Number:</strong> 1016282563</h5>
          <h5><strong>Account Name:</strong> Zenith Bank Plc</h5>
        </div>
      </div>
      <div class="row text3">
        <div class="col-12">
          <h2>After Payment Fill The Registration Form Below</h2>
        </div>
      </div>
      <div class="row">
        <div class="col-md-12">
          <form action="">
            <div class="row">
              <div class="col-md-6">
                <div class="form-group">
                  <label for="name">First Name *</label>
                  <input type="text" class="form-control" placeholder="First Name">
                </div>
              </div>
               <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Last Name *</label>
                  <input type="text" class="form-control" placeholder="Last Name">
                </div>
              </div>
            </div>
             <div class="row">
              <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Email Address *</label>
                  <input type="email" class="form-control">
                </div>
              </div>
               <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Phone Number *</label>
                  <input type="tel" class="form-control">
                </div>
              </div>
            </div>
             <div class="row">
              <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Investment Amount Paid *</label>
                  <input type="number" class="form-control" placeholder="Type in only numbers">
                </div>
              </div>
               <div class="col-md-6">
                <div class="form-group">
                  <label for="name">Where should we pay your earnings *</label>
                  <input type="tel" class="form-control" placeholder="Acc. Name, Acc. Number, Bank Name">
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col-12">
                <label for="upload">Upload your proof of payment *</label>
               <div class="form-group">
                  <input type="file" name="" id="">
               </div>
              </div>
            </div>
            <div class="row">
              <div class="col-12">
                <div class="form-group">
                  <label for="">What address should be in your MOU/Contract Agreement? *</label>
                  <input type="text" class="form-control">
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col-12">
                <div class="form-group">
                  <label for="">Create a Login Username *</label>
                  <input type="text" class="form-control">
                </div>
              </div>
            </div>
             <div class="row">
              <div class="col-12">
                <div class="form-group">
                  <label for="">Create a Login Password *</label>
                  <div class="row">
                    <div class="col-md-6">
                      <input type="text" class="form-control">
                      <small id="passwordHelpBlock" class="form-text text-muted">Create a login password </small>
                    </div>
                     <div class="col-md-6">
                      <input type="text" class="form-control">
                      <small id="passwordHelpBlock" class="form-text text-muted">Confirm your login password </small>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col-12 text-center">
                <div class="strengh">
                  Strenght Indicator
                </div>
              </div>
            </div>
            <button type="submit" class="register__btn">Submit</button>
          </form>
        </div>
      </div>
     </div>
    </div>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue';
import Footer from '@/components/Footer.vue';
export default {
  components:{
    Navbar,
    Footer
  }
}
</script>
<style lang="scss" scoped>
@import '../assets/styles/_colors';
.heading__wrapper{
  background: $secondary-color;
  padding: 6rem 0;
  color: #fff;
  h1{
    font-weight: 800;
    color: #ffff00;
    font-size: 4rem;
    text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,0.3);
    padding-bottom: 1rem;
  }
  p{
    font-size: 1.1rem;
    opacity: .98;
  }
  p::after {
	content: "";
	width: 180px;
	position: absolute;
	margin: 0 auto;
	height: 7px;
	background: #fff;
	left: 0;
	right: 0;
  bottom: -25px;
}
}

.intro__section{
  padding: 4rem 0;
  .text1{
    h5{
      padding-bottom: 1.5rem;
      line-height: 1.6;
      font-size: 1.14rem;
      color: #333;
      opacity: .85;
    }
  }
  .text2{
    padding-bottom: 1.5rem;
    padding-top: .5rem;
    h4{
      color: #008e51;
      font-weight: bolder;
      padding-bottom: .5rem;
    }
    h5{
      font-size: 1.1rem;
      line-height: 1.5;
      color: #333;
      opacity: .7;
    }
    // .title{
    //   color: #333;
    //   font-weight: bold;
    //   opacity: .85;
    //   font-size: 1rem;
    // }
  }
  .text3{
    background: #008E51;
    // padding: .8rem 1rem;
    color: #fff;
    font-weight: bolder;
    margin-bottom: 2rem;
    margin-top: 1rem;
    h2{
      font-weight: bolder;
      text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,0.5);
      font-size: 2.2rem;
      padding-top: .8rem;
      padding-bottom: .7rem;
    }
  }
  form{
    label{
      font-size: 1rem;
      color: #333;
      font-weight: bold;
      opacity: .8;
    }
    input{
      height: 3rem;
      box-shadow: none;
      border-radius: 0px;
    }
    .strengh{
      background: #EEEEEE;
      padding: 1rem;
      margin-bottom: 2rem;
      border-bottom: 2px solid #ccc;
    }
    .register__btn{
      background: #008E51;
      color: #fff;
      padding: 1rem 5rem;
      border-radius: 0px;
      text-decoration: none;
      // border: none
      font-weight: 400;
    }
  }
}

//MEIDA QUERIES
@media only screen and (max-width: 600px){
  .heading__wrapper{
    padding: 6rem 0;
    h1{
      padding: 0 .5rem;
      font-size: 2.5rem;
      font-weight: bolder !important;
      padding-bottom: 1rem;
    }
  }
  .intro__section{
    .text3{
    margin: 0 .3rem !important;
    h2{
      font-size: 1.4rem !important;
      line-height: 1.5;
    }
  }
  }
  form{
    margin-top: 2rem !important;
  }
}
</style>