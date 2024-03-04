<script lang="ts">
    import Saos from "saos";
</script>


<div class="flex flex-row w-full p-4 gap-x-4">

    <!-- <div class="w-full"> -->
        <Saos once={true} animation={"from-left 1.5s cubic-bezier(0.35, 0.5, 0.65, 0.95)"} css_observer="width:100%">
            <div class="bg-purple-500 w-full h-[500px] flex items-center justify-center">
                div 1 - trigger once
            </div>
        </Saos>
    <!-- </div> -->
    
    <div class="bg-red-500 w-full h-[500px] flex items-center justify-center">
        div 2
    </div>

</div>

<div>
    a<br>a<br> a<br>a<br>a<br>a<br>a<br>a<br> a<br>a<br>a<br>a<br> 
</div>

<div class="flex flex-row w-full p-4 gap-x-4">

    <div class="bg-blue-500 w-full h-[500px] flex items-center justify-center">
        div 1
    </div>

    <div class="w-full">
        <Saos animation={"from-left 1.5s cubic-bezier(0.35, 0.5, 0.65, 0.95) both"}>
            <div class="bg-yellow-500 w-full h-[500px] flex items-center justify-center">
                div 2 - trigger multiple time
            </div>
        </Saos>
    </div>

</div>


<style>
    @keyframes -global-from-left {
        0% {
            transform: rotateX(50deg) translateX(-200vw) skewX(-50deg);
            opacity: 1;
        }
        100% {
            transform: rotateX(0deg) translateX(0) skewX(0deg);
            opacity: 1;
        }
    }

    @keyframes -global-rotate-center {
        0% {
            -webkit-transform: rotate(0);
                    transform: rotate(0);
        }
        100% {
            -webkit-transform: rotate(360deg);
                    transform: rotate(360deg);
        }
    }

</style>