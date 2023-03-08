
 <template>

    <nav class="md:flex justify-between items-center">
        <div class="flex md:block justify-between items-center">
            <div class=""><img src="../assets/images/logo.svg" alt="logo" class=""/></div>
            <span  @click="openMenu()"  class=" bg-black md:hidden  cursor-pointer">
                <img v-if="open" src="../assets/images/close.svg" alt="">
                <img v-else src="../assets/images/Hamburger.svg" alt="">
            </span>
        </div>
        <ul class=" py-8 md:py-0  px-8 md:px-0 md:flex-row flex  flex-col gap-4 text-xl md:text-lg font-bold text-white md:text-black  items-center mt-12 md:mt-0 md:static absolute bg-[#0A142F] md:bg-white md:w-auto w-[90%] h-fit md:h-auto rounded-2xl duration-500 ease-in" :class="[open ? 'left-[1rem]' : '-left-full']">
            <li>Features</li>
            <li>Pricing</li>
            <li>Resources</li>
        </ul>

    </nav>

        <div  class="">
            <slot/>
        </div>
</template>

<script >
import { ref } from 'vue'

export default {

    setup(){

        let open = ref(false)

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















