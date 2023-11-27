<template>
    <div>
        <header>
            <nav class="navbar">
                <div class="navbar__logo">
                    <img
                        src="https://media.discordapp.net/attachments/1042442013510991962/1178783334306951168/photo_5359526415952893947_y.jpg?ex=65776687&is=6564f187&hm=3039c839fe914253d3691a2d2748764fe9c5c8fdf4a8dbe0fe4f0e0f558a12ab&=&format=webp&width=343&height=671">
                </div>


                <ul class="navbar__list">
                    <li><a href="#" class="navbar__List-link">Главная</a></li>
                    <li><a href="#" class="navbar__List-link">Магазин</a></li>
                    <li><a href="#" class="navbar__List-link">Отзывы</a></li>
                </ul>

                <ul class="navbar__social">
                    <li><a href="#" class="navbar__soical-link">
                            <i class="fa-brands fa-telegram"></i>
                        </a></li>
                    <li><a href="#" class="navbar__soical-link">
                            <i class="fa-brands fa-vk"></i>
                        </a></li>
                    <li><a href="#" class="navbar__soical-link">
                            <i class="fa-brands fa-discord"></i>
                        </a></li>
                </ul>
            </nav>
            <div class="line-wrapper">
                <div class="navbar__line">
                    <hr>
                </div>
            </div>

        </header>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.navbar {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    gap: 30px;
    padding: 16px;

    &__logo {
        img {
            border-radius: 50%;
            width: 64px;
            height: 64px;
        }
    }

    &__list,
    &__social {
        display: flex;
        flex-direction: row;
        gap: 30px;
        align-items: center;

    }

}


.navbar__List-link {
    font-size: 1.25rem;
    color: black;
    font-weight: 600;

    transition: all 0.5s;

    &:hover {
        font-weight: 700;
    }
}

.navbar__soical-link>i {
    font-size: 1.05rem;
    color: black;
    transition: transform 0.3s;

    &:hover {
        font-size: 1.20rem;
        color: rgb(0, 0, 0);
        transform: rotate(180deg);
    }
}


.line-wrapper {
    display: flex;
    justify-content: center;
    margin-bottom: 2rem;
}

.navbar__line {
    width: 100%;
    max-width: 500px;
    height: 3px;
    background-color: black;
    border-radius: 6px;
    /* остальные стили */
}
</style>