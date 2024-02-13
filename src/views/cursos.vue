<script setup>

</script>
<template>
    <section>
        <h1 class="title-e">Cursos y Certificaciones</h1>
    <div class="tarjeta-cursos">
        <ul class="trg">
            <li class="tarjeta-c">
                <img src="../assets/infotec.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Full-Stack</h1>
                    <h2>Infotec 2022</h2>                    
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Udemy.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Vue js 3, Vite, Firebase 9.</h1>
                    <h2>Udemy 2022</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Google.webp" loading="lazy" alt="curso">
                <div class="card-curso">
                    <h1>HTML y CSS</h1>
                    <h2>Google Activate 2022</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Linkedin.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Web Full-Stack</h1>
                    <h2>Linkedin 2022</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Microsoft.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Formacion de Developers</h1>
                    <h2>Microsoft y LaunchX 2022</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Linkedin.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Administracion de Redes</h1>
                    <h2>Linkedin 2021</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Udemy.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Sistemas Ecommerce Bootstrap HTML5 CSS3 JS php JSON API</h1>
                    <h2>Udemy 2020</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/Google.webp" loading="lazy" alt="udemy">
                <div class="card-curso">
                    <h1>Marketing digital</h1>
                    <h2>Google 2018</h2>
                </div>                
            </li>
            <li class="tarjeta-c">
                <img src="../assets/conversa.jpg" alt="udemy">
                <div class="card-curso">
                    <h1>Formación de instructores de informática</h1>
                    <h2>Udemy 2017</h2>
                </div>                
            </li>
        </ul>
    </div>
    </section>
</template>
<style>
    .title-e{
        font-size: 2.9rem;
        margin-top: 2rem;
        margin-bottom: 5rem;
        color: var(--colortexto);
    }
    .tarjeta-cursos{       
        background-color: white;
        border-radius: .5rem;
        padding: 2rem;
    }
    .trg{
        display: grid;
        grid-template-columns: repeat(3, 3fr);
        gap: 2rem;
    }
    .tarjeta-c{
        display: grid;
        grid-template-columns: 2fr 8fr;
        gap: 1rem;
        align-items: center;
        font-size: .5rem;
    }

    .card-curso{
        /*Linea debajo marcada*/
        border-bottom: 1px solid #dadada;
    }
    .card-curso h1{
        font-size: 1rem;
        margin-bottom: .1rem;
    }
    .card-curso h2{
        font-size: .8rem;
        font-weight: 700;
        color: #747474;
    }
    @media (max-width: 575px) {
        .trg{
        display: grid;
        grid-template-columns: repeat(1, 1fr);
        gap: 2rem;
        }
        .title-e{
        font-size: 2rem;
        margin-top: 2rem;
        margin-bottom: 5rem;
        color: var(--colortexto);
        text-align: center;
        padding: 1rem;
        }
        .tarjeta-cursos{  
            padding:.5rem;
        }
    }
</style>