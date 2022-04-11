<script setup>

import heroImage from './assets/sailor-moon.jpg'

</script>

<script>
export default {

}
</script>

<template>
  <main id="main">
    <h1 id="title">Sailor Moon</h1>
    <h2>¡Te castigaré en nombre de la justicia y el amor!</h2>
    <figure id="img-div">
      <img id="image" :src="heroImage" alt="5 sailor moon">
      <figcaption id="img-caption">Las 5 guerreras</figcaption>
    </figure>
    <section>
      <h3 id="tribute-info">Cronología de las temporadas de Guerrera Luna</h3>
      <ul>
        <li><span class="item-year">1992</span> Se estrena Sailor Moon. Una niña torpe y miedosa cambia su vida de forma
          radical cuando se
          encuentra con una gata parlante llamada <em>Luna</em></li>
        <li><span class="item-year">1993</span> Han pasado 2 meses desde el final de la batalla contra el Reino Oscuro.
          Las 5 chicas, y Mamoru (Tuxido Mask), que resucitaron gracias al milagroso poder del Cristal de Plata viven
          ahora como cualquier joven sin ningún recuerdo de todo lo que les ocurrió. Usagi (Serena) sigue siendo alegre
          y torpe, y Mamoru (Darien) sigue burlándose de ella. </li>
        <li><span class="item-year">1994</span> Las chicas tienen problemas con los estudios pues se acerca el momento
          de dar su examen de admisión a la preparatoria. Rei se encuentra preocupada debido a una pesadilla recurrente
          en que ve cómo todo, incluyendo las Sailors, es destruido por completo. </li>
      </ul>
    </section>
    <a id="tribute-link" href="https://es.wikipedia.org/wiki/Anexo:Episodios_de_Sailor_Moon#Sailor_Moon_S_(090-127)"
      target="_blank">Fuente: Wikipedia, episodios de Sailor Moon</a>
  </main>

</template>

<style>
@import './assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

figure {
  border: thin #c0c0c0 solid;
  display: flex;
  flex-flow: column;
  padding: 5px;
  margin: auto;
}

img {
  max-width: 100%;
}

figcaption {
  background-color: #222;
  color: #fff;
  font-style: italic;
  font-weight: 700;
  padding: 3px;
  text-align: center;
}

header {
  line-height: 1.5;
}

.item-year {
  font-weight: bold;
}

.item-year::after {
  content: ':';
  font-weight: bold;

}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

@media (min-width: 1024px) {
  body {
    display: flex;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 2rem;
  }
}
</style>
