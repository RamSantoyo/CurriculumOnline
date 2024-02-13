<script setup>

</script>

<template>
    <section>
        <div class="informacion">
            <img src="../assets/laptop.webp" loading="lazy" alt="laptop"> 
            <div class="parrafo-info">
                <h1 class="title">Sobre mi...</h1>
                <p>Hola soy Ramsess, durante este tiempo me he estado especializando como <strong>Front End Developer</strong> y he tenido la oportunidad de trabajar en proyectos de desarrollo web, en los cuales he podido aplicar y ampliar mis conocimientos, aquí encontrarás algunos de mis proyectos.</p>
            </div>           
        </div>        
    </section>
</template>

<style>
    .informacion{
        display: grid;
        grid-template-columns: repeat(2, 2fr);
        gap: 2rem;
        margin-top: -4rem;
    }
    .parrafo-info h1{
        font-size: 2.5rem;
        font-weight: var(--grande900);
    }

    .parrafo-info p{
        font-size: 1.3rem;
        text-align: center;
    }

    @media (max-width: 575px) {
        .informacion{
        display: grid;
        grid-template-columns: repeat(1, 1fr);
        }
    }

</style>