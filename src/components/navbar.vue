<!-- <template>
    <nav class="flex items-center justify-between "> 
        <div class="flex items-center justify-between gap-6" >
            <img src="../assets/images/logo.svg" alt="logo">
            <ul class="flex items-center justify-between gap-4">
                <li>Features</li>
                <li>Pricing</li>
                <li>Resources</li>
            </ul>
        
        </div>

        <div class="flex items-center justify-between gap-4">
            <button>Login</button>
            <button>Sign Up</button>
        </div>

    </nav>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style> -->

<!-- <template>
<nav class="navbar">
    <div class="navbar-brand">
    <img class="navbar-logo" src="../assets/images/logo.svg" alt="Logo">
    </div>
    <div class="navbar-menu " :class="{'show': isMenuOpen}">
    <a href="#" class="navbar-item">Home</a>
    <a href="#" class="navbar-item">About</a>
    <a href="#" class="navbar-item">Contact</a>
    </div>
    <button @click="isMenuOpen = !isMenuOpen" type="button" class="navbar-toggle" :class="{'active': isMenuOpen}">
    <span class="navbar-toggle-icon"></span>
    </button>
</nav>
</template>
  
<script>
export default {
data() {
    return {
    isMenuOpen: false,
    };
},
};
</script>
  
<style lang="scss">

  .navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #fff;
    padding: 1rem;
    //box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  
    .navbar-brand {
      .navbar-logo {
        height: 2rem;
      }
    }
  
    .navbar-menu {
      display: flex;
      flex-direction: column;
      position: absolute;
      background-color: #fff;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s ease-in-out;
      transform: translateX(100%);
      z-index: 10;
      padding: 1rem;
  
      .navbar-item {
        padding: 0.5rem;
        border-radius: 0.25rem;
        font-size: 1.125rem;
        color: #333;
        text-decoration: none;
        transition: background-color 0.2s ease-in-out;
  
        &:hover {
          background-color: #f2f2f2;
        }
      }
    }
  
    .navbar-toggle {
      appearance: none;
      background-color: transparent;
      border: none;
      cursor: pointer;
      padding: 0;
      width: 2rem;
      height: 2rem;
      position: relative;
      z-index: 20;
  
      .navbar-toggle-icon {
            position: absolute;
            left: 0.25rem;
            top: 0.25rem;
            width: 1.5rem;
            height: 1.5rem;
            background-color: #333;
            border-radius: 0.25rem;
            transition: transform 0.2s ease-in-out;

            &::before,
            &::after {
                content: "";
                position: absolute;
                left: 50%;
                top: 50%;
                width: 1rem;
                height: 0.125rem;
                background-color: #fff;
                transform: translate(-50%, -50%);
                transition: transform 0.2s ease-in-out;
            }

            &::before {
                transform: translate(-50%, -50%) rotate(-45deg);
            }

            &::after {
                transform: translate(-50%, -50%) rotate(45deg);
            }
        }
  
    &.active .navbar-toggle-icon {
        transform: rotate(45deg);

        &::before {
            transform: translate(-50%, -50%) rotate(135deg);
        }

        &::after {
            transform: translate(-50%, -50%) rotate(-135deg);
        }
    }

    }

    @media (min-width: 768px) {
        .navbar-menu {
            position: static;
            flex-direction: row;
            background-color: transparent;
            box-shadow: none;
            transform: none;
            padding: 0;
        
          .navbar-item {
            margin-right: 1rem;
        
            &:last-child {
              margin-right: 0;
            }
          }
        }
        
        .navbar-toggle {
          display: none;
        }
    }
}

</style>
 -->

 <template>
    <div>
        <header class=" px-4 md:px-[50px] py-6 text-white ">

            <nav class="md:flex justify-between items-center">
                <div class="flex md:block justify-between items-center">
                    <div class=""><img src="../assets/images/logo.svg" alt="logo" class="md:w-4/5"/></div>
                    <span @click="openMenu()"  class=" md:hidden  cursor-pointer">
                        <p class="text-black">ll</p>
                        <!-- <img v-if="open" src="../assets/images/close.svg" alt="">
                        <img v-else src="../assets/images/Hamburger.svg" alt=""> -->
                    </span>
                </div>
                <ul class="  px-8 md:px-0 block md:flex text-xl md:text-lg  items-center mt-8 md:mt-0 md:static absolute bg-[#0A142F] md:w-auto w-full h-screen md:h-auto duration-500 ease-in" :class="[open ? 'left-0' : '-left-full']">
                    <li ><a href="#home">Home</a></li>
                    <li class="md:ml-6 my-6 md:my-0"><a href="#services">Our services</a></li>
                    <li class="md:ml-6 my-6 md:my-0"><a href="#about">About Us</a></li>
                    <li class="md:ml-6 my-6 md:my-0"><a href="#projects">Projects</a></li>
                </ul>
                <a href="#footer" class="btn hidden md:flex">Contact Us</a>
            </nav>
        </header>

        <div  class="">
            <slot/>
        </div>

    </div>
</template>

<script >
import { ref } from 'vue'

export default {

    setup(){

        let open = ref(false)

        console.log(open.value);

        function openMenu(){
            open.value = !open.value
        }
        

        return{
            open,
            openMenu
        }

    }
}




</script>

<style lang="scss" scoped>


</style>















