<template>
    <nav class="nav-menu">
        <div class="nav-mobile">
            <i class="fal fa-ellipsis-v" @click="mostrarMenu()"></i>
            <a class="logo" href="#">
                <img src="@/assets/svg/logo.svg" alt="Logo" />
            </a>
            <div></div>
        </div>
        <div class="nav-conteudo" :class="this.exibirMenuMobile ? 'menu-aberto' : 'menu-fechado'">
            <div class="logo">
                <a href="#">
                    <img src="@/assets/svg/logoENome.svg" alt="Logo" />
                </a>
            </div>
            <ul class="nav-items">
                <li><a href="#">ABOUT US</a></li>
                <li><a href="#">MODELS</a></li>
                <li><a href="#">GUARANTEE</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: "Navbar",
    data() {
        return {
            exibirMenuMobile: false,
        };
    },
    methods: {
        mostrarMenu() {
            this.exibirMenuMobile = !this.exibirMenuMobile;
        },
    }
};
</script>

<style lang="scss" scoped>
.nav-menu {
    background-color: white;
}

a,
a:link,
a:visited,
a:focus,
a:hover,
a:active {
    color: #846219;
}

.nav-conteudo {
    padding: 10px 30px;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .nav-items {
        flex-grow: 1;
    }

    .logo {
        flex-grow: 1;
    }
}

.logo img {
    height: 50px;
}

.nav-items {
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
    list-style: none;
    margin: 0;
    padding: 0;

    li {
        padding: 0 10px;
    }
}

.nav-mobile {
    display: none;
}

/* Mobile version */
@media screen and (max-width: 768px) {
    .nav-menu {
        position: absolute;
        width: 100%;
    }

    .menu-aberto {
        opacity: 1;
        height: 150px;
    }

    .menu-fechado {
        opacity: 0;
        height: 0;
        padding: 0;
    }

    .nav-conteudo {
        flex-direction: column;
        z-index: 100;
        position: relative;
        transition: all 0.2s ease-out;
        
        div.logo {
            display: none;
        }
    }

    .nav-items {
        flex-direction: column;
        align-items: center;
    }

    .nav-mobile {
        display: flex;
        padding: 5px 20px 10px 20px;
        height: 50px;
        justify-content: space-between;
        align-items: center;

        i {
            font-size: 40px;
            color: #E2E0B8;
        }
    }
}
</style>