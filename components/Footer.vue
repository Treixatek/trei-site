<template>
    <footer>
        <div class="logoFoot">
            
        </div>
        <div class="bottom">
            <p><span style="color: #5e6978">© 2020 by Treixatek LLC. All Rights Reserved</span></p>
            <p class="rightSide"><span style="color: #5e6978">Privacy Policy</span></p>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style>
    footer {
        background-color: #38404f;
        box-shadow: 0px -2px 5px rgba(0,0,0,0.6);
    }

    .logoFoot {
        width: 100%;
        height: 100px;
        padding-top: 10%;
        
    }
    .bottom {
        display: grid;
        grid-template-columns: repeat(2, auto);
        background-color: #2c3040;
        width: 100%;
        padding-top: 1%;

        padding: 1%;
    }
    .rightSide {
        position: absolute;
        right: 2%;

        
    }
</style>