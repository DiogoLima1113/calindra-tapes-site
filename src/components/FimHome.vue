<template>
    <section class="container">
        <div class="texto">
            
            <div class="titulo">
                <div>We are Leader</div>
                <div>in Measure Tapes</div>
            </div>
            <div class="subtitulo">
                <div>There are 5x the</div>
                <div>circumference of planet</div>
                <div>earth in metric tapes.</div>
            </div>
        </div>
        <img class="logo" src="@/assets/svg/fitaEsticada.svg" alt="Fita Esticada" />
    </section>
</template>
  
<script>

export default {
    name: 'FimHome',
};
</script>
  
<style lang="scss" scoped>
section.container {
    height: 100vh;
    background-color: #506FA9;
    color: #FFFFFF;
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

.titulo {
    font-weight: bold;
    font-size: 5vw;
}

.subtitulo {
    font-size: 3vw;
    font-weight: 300;
}

img {
    mix-blend-mode: multiply;
}

.texto {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    gap: 55px;
    height: 100%;
    position: absolute;
    top: 88%;
    left: 11%;
}


/* Mobile version */
@media screen and (max-width: 768px) {
    section.container {
        padding-left: 15px;
        flex-direction: column;
        align-items: flex-end;
        justify-content: center;
        gap: 35px;
    }

    .titulo {
        font-size: 12vw;
    }

    .subtitulo {
        font-size: 8vw;
    }

    .texto {
        position: static;
        gap: 35px;
        align-self: flex-start;
        height: 40%;
    }

    img {
        width: 80%;
    }
}
</style>