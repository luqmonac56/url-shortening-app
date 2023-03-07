<template>
    <footer class=" py-8 lg:flex text-center lg:text-left justify-between lg:px-[5rem] bg-[#35323e] text-white">
        <div >
            <img class="mx-auto mt-0 mb-[3rem]" src="../assets/images/whitelogo.svg" alt="">
        </div>
        <div class=" flex flex-col  lg:flex-row mb-12 lg:mb-0 gap-12 justify-between">
            <ul class="flex flex-col gap-4">
                <li class="font-bold mb-2">Features</li>
                <li>Link Shortening</li>
                <li>Branded Links</li>
                <li>Analysis</li>
            </ul>
            <ul class="flex flex-col gap-4">
                <li class="font-bold mb-2">Features</li>
                <li>Link Shortening</li>
                <li>Branded Links</li>
                <li>Analysis</li>
            </ul>
            <ul class="flex flex-col gap-4">
                <li class="font-bold mb-2">Features</li>
                <li>Link Shortening</li>
                <li>Branded Links</li>
                <li>Analysis</li>
            </ul>
        </div>
        <div class=" grid-logo w-1/2 max-w-[190px] mx-auto my-0 lg:mx-0  ">
            <div><img class="" src="../assets/images/icon-facebook.svg" alt="icon-facebook"></div>
            <div><img class="" src="../assets/images/icon-instagram.svg" alt="instagram"></div>
            <div><img class="" src="../assets/images/icon-twitter.svg" alt="twitter"></div>
            <div><img class=" " src="../assets/images/icon-pinterest.svg" alt="pintrest"></div>
        </div>
    </footer>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.grid-logo{
    display: flex;
    //display: grid;
    //grid-template-columns: repeat(4, 1fr);
    //grid-template-rows: 1fr;
    gap: 1rem;

    div{
        margin: 0 auto;
    }
}

</style>