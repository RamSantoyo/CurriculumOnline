<script setup>

</script>
<template>
    <div>
        <div class="front">
            <h1 class="title">Front End</h1>
            <h1 class="title2">Developer</h1>
        </div>
        <p class="parrafo">Bienvenido a mi portafolio, aquí encontrarás algunos de mis proyectos.</p>
    </div>
    <div>
        <img class="foto" src="../assets/profile.webp" loading="lazy" alt="foto">        
    </div>
</template>
<style>
    .front{
        display: flex;
        justify-content: center;
        gap: .5rem;
    }
    .title, .title2{
        text-align: center;
        font-size: 1.5rem;
        font-weight: 100;
    }
    .title2{
        color: var(--colorterceario);
    }
    .parrafo{
        text-align: center;
        font-size: 4rem;
        margin: 0rem;
    }

    .foto{
        margin: 2rem auto;
        width: 50%;
    }
    @media (max-width: 575px) {
    
    .parrafo{
        text-align: center;
        font-size: 2.5rem;
        margin: 0rem;
    }
    .foto{
        margin: 2rem auto;
        width: 100%;
    }
}
</style>