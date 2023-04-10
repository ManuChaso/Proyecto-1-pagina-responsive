# Proyecto 1: Página web responsive.
### Replica de la tienda de Heretics

He replicado la tienda de un Equipo de Esports llamado Heretics. [Link a la página original](https://teamheretics.com/21-store).

Quiero aclarar que la animación del "home" se la pedí a Chatgpt, soy capaz de hacerla, pero justo andaba probando cosas y me dio por intentarlo a ver que salía. Esta es la parte concreta que hizo Chatgpt:

*HTML*
```HTML
<div class="home">
        <img src="https://teamheretics.com/modules/revsliderprestashop/uploads/safasf/new-pro-kit-banner-1920x700.png" alt="Imagen 1">
        <img src="https://teamheretics.com/modules/revsliderprestashop/uploads/Drop%20BelaguerXHeretics%20-%20Banner%20web.png" alt="Imagen 2">
        <img src="https://teamheretics.com/modules/revsliderprestashop/uploads/safasf/bufanda-oficial-banner.png" alt="Imagen 3">
</div> 
```

*CSS*

```CSS
.home {
    position: relative;
    width: 100%;
    height: 550px;
    overflow: hidden;
}

.home img {
    position: absolute;
    width: 100%;
    height: 100%;
    opacity: 0;
    animation-name: fade;
    animation-duration: 12s;
    animation-timing-function: ease-in-out;
    animation-iteration-count: infinite;
}
      
.home img:nth-child(1) {
    animation-delay: 0s;
}
      
.home img:nth-child(2) {
    animation-delay: 4s;
}
      
.home img:nth-child(3) {
    animation-delay: 8s;
}
      
@keyframes fade {
    0% {
        opacity: 0;
    }
    25% {
        opacity: 1;
    }
    75% {
        opacity: 1;
    }
    100% {
        opacity: 0;
    }
}
```

También aclarar que he decidido separar el CSS en dos archivos (Escritorio y móvil) porque me parecía mas organizado. 