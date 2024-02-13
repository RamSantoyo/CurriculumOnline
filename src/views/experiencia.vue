<script setup>


</script>
<template>
    <h1 class="title-e">Experiencia</h1>
    <div class="contenedor-acordeon">
        <div class="tarjeta-exp">        
            <button class="accordion">
                <img src="../assets/infotec.webp" loading="lazy" alt="logo">
                <div class="cnt-acordion">
                    <h1>Full-Stack</h1>
                    <p>Practicante Desarrollo Web</p>
                    <p class="año">2022-2023 (4 meses)</p>
                </div>
            </button>
            <div class="panel">
                <p>Desarrollo de paginas web con HTML, CSS, JavaScript, Java, Bootstrap, Angular, Git, Github asi como el manejo de la metodologia SCRUM con Dayli Meetings, Sprint Planning, Sprint Review y Sprint Retrospective.</p>
            </div>
        </div>
        <div class="tarjeta-exp">        
            <button class="accordion">
                <img src="../assets/ids.webp" loading="lazy" alt="logo">
                <div class="cnt-acordion">
                    <h1>Front End Jr</h1>
                    <p>Becario Front End</p>
                    <p class="año">2022 (3 meses)</p>             
                </div>
            </button>
            <div class="panel">
                <p>Como becario Front End maquetando y desarrollando paginas web utilizando Vuejs, Vite, HTML, CSS, JavaScript, Git, Github, buenas practicas de programacion y desarrollando componentes reutilizables.</p>
            </div>
        </div>
    </div>
</template>
<style>
    button{
        border: none;
    }
    .tarjeta-exp{
        margin-bottom: 4rem;
    }
    .accordion{
        display: grid;
        grid-template-columns: 1fr 9fr;
        align-items: center;
        background-color: var(--colorfondo);
        cursor: pointer;        
    }
    .cnt-acordion{
        text-align: left;
        padding-left: 2rem;
        line-height: 50%;
    }
    .cnt-acordion p{
        color: rgb(131, 131, 131);
    }
    
    .panel{
        padding-left: 10rem;
    }
    .contenedor-acordeon{
        margin: 2rem;
    }
    .panel{
        line-height: 1.5rem;
    }
    .año{
        color: var(--colorterceario) !important;
    }

    @media (max-width: 575px) {
        .accordion{
        display: grid;
        grid-template-columns: repeat(1, 1fr);
        align-items: center;
        background-color: var(--colorfondo);
        cursor: pointer;        
    }
    .panel{
        padding: 1rem;
        text-align: center;
    }
    .accordion img{
        width: 60%;
        margin: 0 auto;
    }
    }
    
</style>