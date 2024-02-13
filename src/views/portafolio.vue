<script setup>

</script>
<template>
    <div>
        <h1 class="title-e">Portafolio</h1>
    </div>
    <div class="cnt-tarjetas-prt">

        <a href="https://lucid-jennings-0f3196.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-1.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Bienes Raices</h2>
        </a>
        <a href="https://laughing-khorana-05f658.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-2.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Cafeteria</h2>
        </a>
        <a href="https://hardcore-mestorf-c18b25.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-3.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Blog</h2>
        </a>
        <a href="https://ecstatic-shirley-cbd3cd.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-4.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Barberia</h2>
        </a>
        <a href="https://hopeful-sammet-a178db.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div>
                        <img class="img" loading="lazy" src="../assets/porta-5.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Api Rest</h2>
        </a>
        <a href="https://wizardly-torvalds-9788b8.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-6.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Landing Page</h2>
        </a>
        <a href="https://merry-blini-7bca0b.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" src="../assets/porta-7.jpg" alt="">
                    </div>                
                </div>            
            </div>
            <h2>Login</h2>
        </a>
        <a href="https://deft-sorbet-3fe892.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-8.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Buscador</h2>
        </a>
        <a href="https://helpful-cannoli-f764a8.netlify.app/" target="_blank">
            <div class="card">
                <div class="imgbox">
                    <div >
                        <img class="img" loading="lazy" src="../assets/porta-9.webp" alt="proyecto">
                    </div>                
                </div>            
            </div>
            <h2>Divisas</h2>
        </a>
    </div>
</template>
<style>
a{
    text-decoration: none;
    color: black;
}
.cnt-tarjetas-prt{
    display:grid;
    grid-template-columns: repeat(3, 1fr);
    margin-bottom: 5rem;
}
.card {
  overflow: visible;
  position: relative;
  width: 18rem;
  height: 25rem;
  background: #fff;
  box-shadow: 0 2px 10px rgba(0, 0, 0, .2);
  margin-top: 1rem;
}

.card:before,
.card:after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 4px;
  background: #fff;
  transition: 0.5s;
  z-index: -99;
}

/*Image*/
.imgbox {
  position: absolute;
  top: 10px;
  left: 10px;
  bottom: 10px;
  right: 10px;
  background: #222;
  transition: 0.5s;
  z-index: 1;
}

.img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

/*Hover*/
.card:hover .imgbox {
  cursor: pointer;
  bottom: 11px;
}

.card:hover:before {
  transform: rotate(20deg);
}

.card:hover:after {
  transform: rotate(10deg);
  box-shadow: 0 2px 20px rgba(0, 0, 0, .2);
}

@media (max-width: 575px) {
    .cnt-tarjetas-prt{
        display:grid;
        grid-template-columns: repeat(1, 1fr);
        margin: 0 auto;
    }
}
</style>