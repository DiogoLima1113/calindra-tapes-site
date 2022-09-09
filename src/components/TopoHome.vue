<template>
    <section class="container">
        <div>
            <div>Measuring</div>
            <div>everything</div>
        </div>
        <img class="logo" src="@/assets/svg/fitaEnrolada.svg" alt="Fita Enrolada" />
    </section>
</template>
  
<script>

export default {
    name: 'TopoHome',
};
</script>
  
<style lang="scss" scoped>
section.container {
    height: 100vh;
    background-color: #E9E9E9;
    color: #716565;
    font-weight: bold;
    font-size: 5vw;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
}

img {
    mix-blend-mode: multiply;
    width: 40vw;
}


/* Mobile version */
@media screen and (max-width: 768px) {
    section.container {
        padding: 30px;
        font-size: 18vw;
        gap: 0px;
        flex-direction: column;

        * {
            align-self: flex-start;
        }

    }

    img {
        width: 100%;
    }
}
</style>