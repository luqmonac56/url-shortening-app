

<template>
  <section class="flex flex-col-reverse lg:flex-row mt-6 lg:pl-12 items-center justify-between">
    <div class=" lg:flex-[1] w-full p-4 lg:p-0 text-center lg:text-left">
      <h1 class=" text-4xl font-bold lg:text-6xl">More than just shorter links</h1>
      <p class="lg:w-[80%]  mt-6 text-[#9e9aa7]">Build your brand's recognition and get detailed insights on how your links are performing.</p>
      <button class=" mt-8 rounded-full px-6 py-2 bg-[#2acfcf] text-white">Get Started</button>
    </div>
    <div class=" flex-[1]  pl-4">
      <img class="w-full mr-[-2rem]" src="../assets/images/illustration-working.svg" alt="">
    </div>
  </section>

  <section class="  relative px-4 lg:px-12 pb-[8rem] bg-[#bfbfbf36] mt-[10rem]">
    <div class="input-div px-4 py-8 lg:p-[3.5rem] flex flex-col lg:flex-row gap-4 lg:gap-8 relative -top-[5rem]">
      <input type="url" placeholder="Shorten a link here..." >
      <button class=" py-4 lg:px-8">Shorten it!</button>
    </div>
    <section>
      <h2 class="text-center text-3xl lg:text-5xl font-bold">Advanced Statistics</h2>
      <p class="text-[#9e9aa7] text-center  mt-4">Track how your links are performing accross the web with our advanced statistics dashboard.</p>
      <div class=" lg:flex justify-between items-center  mt-[3rem]">
        <div class="card w-full lg:w-[30%] shadow-2xl">
          <div class=" p-5 bg-[#35323e] w-fit rounded-full relative -top-8">
            <img src="../assets/images/icon-brand-recognition.svg" alt="icon-brand-recognition">
          </div>
          <h3>Brand Recognition</h3>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius blanditiis aliquid odio amet architecto omnis optio doloribus est harum voluptatem.</p>
        </div>
        <div class="card w-full lg:w-[30%] lg:mt-[5rem] shadow-2xl">
          <div class=" p-5 bg-[#35323e] w-fit rounded-full relative -top-8">
            <img src="../assets/images/icon-brand-recognition.svg" alt="icon-brand-recognition">
          </div>
          <h3>Brand Recognition</h3>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius blanditiis aliquid odio amet architecto omnis optio doloribus est harum voluptatem.</p>
        </div>
        <div class="card w-full lg:w-[30%] lg:mt-[10rem] shadow-2xl">
          <div class=" p-5 bg-[#35323e] w-fit rounded-full relative -top-8">
            <img src="../assets/images/icon-brand-recognition.svg" alt="icon-brand-recognition">
          </div>
          <h3>Brand Recognition</h3>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius blanditiis aliquid odio amet architecto omnis optio doloribus est harum voluptatem.</p>
        </div>
      </div>
    </section>
  </section>

  <div class="boost-section px-4 py-[4rem] lg:p-[4rem]">
    <h2 class="text-4xl">Boost your links today</h2>
    <button class="my-0 mx-auto rounded-full w-fit px-6 py-2 bg-[#2acfcf] text-white">Get Started</button>
  </div>
</template>


<script setup>

</script>

<style lang="scss">

  .input-div{
    //margin-top: 3rem;
    //padding: 3.5rem;
    background-color: #35323e;
    background-image: url(../assets/images/bg-shorten-desktop.svg);
    background-size: cover;
    background-position:center;
    background-repeat: no-repeat;
    border-radius: 15px;
    //gap: 2rem;

    input{
      flex: 1;
      padding: 1.2rem ;
      border: none;
      outline: none;
      border-radius: 10px;
    }

    button{
      background: #2acfcf;
      color: #fff;
      border: none;
      outline: none;
      border-radius: 10px;

    }
  }
  .card{
    background: #fff;
    margin: 0 auto;
    //width: 100%;
    max-width: 400px;
    padding: 0 2rem 2rem 2rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;
    position: relative;
    border-radius: 10px;
    //color:  ;
    color: #9e9aa7;
  }

  .boost-section{
    background-color: #35323e;
    background-image: url(../assets/images/bg-boost-desktop.svg);
    background-size: cover;
    background-position:center;
    background-repeat: no-repeat;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    text-align: center;
    color: #fff;
  }
</style>