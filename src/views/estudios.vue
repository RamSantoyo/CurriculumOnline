<script setup>

</script>
<template>
    <section class="sec-1">        
        <div class="cnt-tarjetas">
            <div class="cnt-title-es">
                <h1 class="title-e">Estudios</h1>
                <p class="p-e">A continuación se detallan mis estudios académicos y las habilidades adquiridas durante mi formación.</p> 
            </div>              
            <div class="tarjetas">
                <div class="tarjeta">
                    <img src="../assets/uin.webp" loading="lazy" alt="estudios">
                    <div class="cnt-tarjeta">
                        <p class="cntp">Desarrollo de software, procesos he implementacion.</p>
                        <h1 class="cnt">2018-2021</h1>                        
                        <p class="cnt">Lic. en Ingenieria en Informatica</p>
                    </div>
                </div>
                <div class="tarjeta">
                    <img src="../assets/tvedu.webp" loading="lazy" alt="estudios">
                    <div class="cnt-tarjeta">                        
                        <p class="cntp">Mantenimiento de software, hardware y redes.</p>
                        <h1 class="cnt">Periodo 2018-2018</h1>
                        <p class="cnt">Tec. Sistemas Informaticos</p>
                    </div>
                </div>
                <div class="tarjeta">
                    <img src="../assets/conversa.jpg" alt="estudios">
                    <div class="cnt-tarjeta">                        
                        <p class="cntp">Ofimatica, Diseño, hardware, software y redes.</p>
                        <h1 class="cnt">Periodo 2015-2017</h1>
                        <p class="cnt">Especialidad en Informatica</p>
                    </div>
                </div>
            </div>
            <div></div>
        </div>        
    </section>    
</template>
<style>
    .title-e{
        font-size: 3rem;
        font-weight: var(--grande700);
        color: var(--colortexto);
    }
    .p-e{
        margin-top: -2rem;
    }
    .cnt-tarjetas{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 2rem;
        margin: 2rem 0;
        align-items: center;
    }
    .tarjetas{
        display: grid;
        grid-template-columns: repeat(1, 1fr);
    }
    .tarjeta{
        display: grid;
        grid-template-columns: 2fr 8fr;
        gap: 5rem;
        background-color: white;
        margin: 1rem;
       border-radius: 10px;
       box-shadow: 0 2px 10px rgba(0, 0, 0, .2);
    }
    /*imahen redonda*/
    .tarjeta img{
        border-radius: 100px;
        width: 80px;
        margin-left: 1rem;
        margin-top: .5rem;
    }
    .cnt-tarjeta{
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: .5rem;
        margin-left: -4rem;
        padding: .9rem;
    }
    .cnt-tarjeta h1{
        font-size: .9rem;
        font-weight: var(--regular300);
        color: #6c757d;
    }
    .cntp{
        font-size: 1rem;
        font-weight: var(--grande700);        
        margin: 0;
        color: var(--colortexto);
    }

    .cnt{
        font-size: .9rem;
        font-weight: var(--delgada200);
        margin: 0;
        color: var(--colorterceario);
    }

    @media (max-width: 575px) {
        .tarjetas{
        display: grid;
        grid-template-columns: repeat(1, 1fr);
        }
        .cnt-tarjetas{
        grid-template-columns: repeat(1, 1fr);
        }
        .tarjeta{
            padding: .4rem;
        }
    }
</style>