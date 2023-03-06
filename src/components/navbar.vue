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

<template>
<nav class="navbar">
    <div class="navbar-brand">
    <img class="navbar-logo" src="../assets/images/logo.svg" alt="Logo">
    </div>
    <div class="navbar-menu">
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
      top: 10rem;
      //right: 0;
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

















