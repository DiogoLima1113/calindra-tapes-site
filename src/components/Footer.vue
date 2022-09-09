<template>
    <footer class="footer">
        <div class="follow">
            <span class="titulo">Follow Us</span>
            <div class="icones">
                <a href="#">
                    <span class="fa-stack fa-2x">
                        <i class="fab fa-youtube fa-stack-1x"></i>
                        <i class="fal fa-circle fa-stack-2x"></i>
                    </span>
                </a>
                <a href="#">
                    <span class="fa-stack fa-2x">
                        <i class="fab fa-facebook-f fa-stack-1x"></i>
                        <i class="fal fa-circle fa-stack-2x"></i>
                    </span>
                </a>
                <a href="#">
                    <span class="fa-stack fa-2x">
                        <i class="fab fa-twitter fa-stack-1x"></i>
                        <i class="fal fa-circle fa-stack-2x"></i>
                    </span>
                </a>
            </div>
        </div>
        <div class="contact">
            <span class="titulo">Contact</span>
            <div class="endereco">
                <div>2490 Leisure Lane</div>
                <div>San Luis Obispo</div>
                <div>California</div>
            </div>
        </div>
        <div></div>
        <div></div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
};
</script>

<style lang="scss" scoped>
.footer {
    background-color: #E9E9E9;
    font-weight: bold;
    color: #716565;
    padding: 50px 0;
    display: flex;
    justify-content: space-around;
    align-items: flex-start;
}

a,
a:link,
a:visited,
a:focus,
a:hover,
a:active {
    color: #716565;
}

.titulo {
    font-size: 2vw;
}

.icones {
    font-size: 12px;
    display: flex;
    gap: 20px;
}

.follow,
.contact {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.endereco {
    font-size: 20px;
    font-weight: 300;
}

/* Mobile version */
@media screen and (max-width: 768px) {
    .footer {
        flex-direction: column;
        align-items: center;
        gap: 45px;
        padding-bottom: 0;
    }

    .follow,
    .contact {
        align-items: center;
    }

    .endereco {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .titulo {
        font-size: 9vw;
    }
}
</style>