<template>
  <div class="home">
    <Navbar />
    <div class="heading__wrapper">
      <div class="container">
        <div class="row">
          <div class="col-12 text-center">
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
          <h5><span class="title">Account Name:</span> Africa Development Crowdfund Limited.</h5>
          <h5><span class="title">Account Number:</span> 1016282563</h5>
          <h5><span class="title">Account Name:</span> Zenith Bank Plc</h5>
        </div>
      </div>
      <div class="row payment__header">
        <div class="col-12 text3">
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
  padding: 6rem;
  color: #fff;
  h1{
    font-weight: 800;
    color: $tertiary-color;
    font-size: 3.7rem;
    text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,0.3);
    padding-bottom: 1rem;
  }
  p::after {
	content: "";
	width: 180px;
	position: absolute;
	margin: 0 auto;
	height: 6px;
	background: #fff;
	left: 0;
	right: 0;
  bottom: -30px;
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
    }
  }
  .text2{
    padding-bottom: 1.5rem;
    h4{
      color: $secondary-color;
      font-weight: bolder;
      padding-bottom: .5rem;
    }
    h5{
      font-size: 1.1rem;
      line-height: 1.5;
      color: #333;
    }
    .title{
      color: #333;
      font-weight: bold;
      opacity: .85;
      font-size: 1rem;
    }
  }
  .text3{
    background: #008E51;
    // padding: .8rem 1rem;
    color: #fff;
    font-weight: bolder;
    margin-bottom: 2rem;
    h2{
      font-weight: bold;
      text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,0.3);
      font-size: 2rem;
      padding-top: .7rem;
      padding-bottom: .7rem;
    }
  }
  form{
    label{
      font-size: 1rem;
      color: #333;
      font-weight: 400;
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
      border: none
    }
  }
}
</style>