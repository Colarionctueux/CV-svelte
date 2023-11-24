<script>
  import { onMount } from "svelte";
  import { fade, blur, fly, slide, scale } from "svelte/transition";
  onMount(() => {
    show = true;
  });

  let show = false;
</script>

{#if show}
  <main>
    <h1>NICOLAS ECKMAN</h1>
    <p>
      Actuellement étudiant en BUT informatique<br />
      à L’IUT A de Lille, je suis passionné d’informatique<br />
      et aime apprendre dans tous les domaines.
    </p>
    <div>
      <aside>
        <h2 transition:slide={{ axis:'x', delay:100}}>PROFIL</h2>
        <h3 transition:fade={{ delay:100, duration: 500 }}>Téléphone</h3>
        <p transition:fade={{ delay:100, duration: 500 }}>07 71 85 23 08</p>
        <h3 transition:fade={{ delay:200, duration: 500 }}>E-mail</h3>
        <p transition:fade={{ delay:200, duration: 500 }}>nicolas.eckmanpro@gmail.com</p>
        <h3 transition:fade={{ delay:300, duration: 500 }}>Date de naissance</h3>
        <p transition:fade={{ delay:300, duration: 500 }}>13 mars 2004</p>
        <h3 transition:fade={{ delay:400, duration: 500 }}>Lien github</h3>
        <a href="https://github.com/Colarionctueux"  transition:fade={{ delay:400, duration: 500 }}>Colarionctueux</a>
        <h2 transition:slide={{ axis:'x', delay:400}}>QUALITÉS</h2>
        <ul>
          <li transition:fade = {{delay : 500, duration: 500}}>Serieux</li>
          <li transition:fade = {{delay : 600, duration: 500}}>Travail en équipe</li>
          <li transition:fade = {{delay : 700, duration: 500}}>Adaptation</li>
          <li transition:fade = {{delay : 800, duration: 500}}>Communication</li>
        </ul>
        <h2 transition:slide={{ axis:'x', delay:800}}>LANGUES</h2>
        <ul>
          <li transition:fade = {{delay : 900, duration: 500}}>Français - natif</li>
          <li transition:fade = {{delay : 1000, duration: 500}}>Anglais - B2</li>
          <li transition:fade = {{delay : 1100, duration: 500}}>Allemand - bases</li>
        </ul>
      </aside>
      <article>
        <section>
          <h2 transition:slide={{ axis:'x', delay:350, duration: 600}}>FORMATION</h2>
          <table>
            <tbody>
              <tr transition:fade = {{delay : 300, duration: 500}}>
                <th>Actuellement</th>
                <td><b>BUT Informatique</b><br />IUT de Lille</td>
              </tr>
              <tr transition:fade = {{delay : 400, duration: 500}}>
                <th>2022</th>
                <td><b>Baccalauréat<br />Spécialités Maths - NSI</b><br />Lycée Raymond Queneau</td>
              </tr>
            </tbody>
          </table>
        </section>
        <section class="competences">
          <h2 transition:slide={{ axis:'x', delay:550, duration: 600}}>COMPÉTENCES</h2>
          <div>
            <b transition:fade = {{delay : 500, duration: 500}}>Développement</b>
            <b transition:fade = {{delay : 600, duration: 500}}>Projets</b>
          </div>
          <div transition:blur>
            <div class="images">
              <img
                transition:fade={{ delay: 700, duration: 500 }}
                src="/java.svg"
                alt="logo java"
              />
              <img
                transition:fade={{ delay: 800, duration: 500 }}
                src="/bash.svg"
                alt="logo bash"
              />
              <img
                transition:fade={{ delay: 900, duration: 500 }}
                src="/html.svg"
                alt="logo html"
              />
              <img
                transition:fade={{ delay: 1000, duration: 500 }}
                src="/css.svg"
                alt="logo css"
              />
              <img
                transition:fade={{ delay: 1100, duration: 500 }}
                src="/c.svg"
                alt="logo c"
              />
              <img
                transition:fade={{ delay: 1200, duration: 500 }}
                src="/psql.svg"
                alt="logo psql"
              />
            </div>
            <ul>
              <li transition:fade={{ delay: 700, duration: 500}}>Jeu - Méthode agile, Java</li>
              <li transition:fade={{ delay: 900, duration: 500 }}>SQL - Gestion base de donnée, Requêtage</li>
              <li transition:fade={{ delay: 1100, duration: 500 }}>IHM - Application d'échange linguistique</li>
              <li transition:fade={{ delay: 1200, duration: 500 }}>HTML - Site d'aide au covoiturage</li>
            </ul>
          </div>
        </section>
        <section>
          <h2  transition:slide={{ axis:'x', delay:950, duration: 600}}>EXPÉRIENCE</h2>
          <table>
            <tbody>
              <tr transition:fade = {{delay : 1300, duration: 500}}>
                <th>2022</th>
                <td><b>Agent d'accueil</b><br />Basic-Fit</td>
              </tr>
              <tr transition:fade = {{delay : 1400, duration: 500}}>
                <th>2019</th>
                <td><b>Stage d'observation</b><br />Sogeti - Capgemini</td>
              </tr>
            </tbody>
          </table>
        </section>
      </article>
    </div>
  </main>
{/if}

<style>
  :global(*) {
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  }

  :global(body) {
    display: flex;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0.1);
  }

  main {
    width: 900px;
    height: calc(900px * 1.41);
    background-color: rgb(255, 255, 255);
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
    border-radius: 10px;
  }

  main > * {
    margin-left: 0;
  }

  main h1 {
    margin-left: 1em;
    margin-top: 30px;
    margin-bottom: 0;
    font-size: 3em;
    color: rgb(5, 42, 53);
    padding-top: 3%;
  }

  a {
    color: white;
  }

  main > p {
    background: linear-gradient(to top, rgb(11, 73, 167), rgb(1, 71, 221));
    padding: 25px;
    padding-left: 1em;
    padding-right: 0;
    width: 70%;
    font-size: 1.7em;
    margin-bottom: 35px;
    margin-top: 35px;
    color: white;
    border-radius: 0 5px 5px 0;
  }

  aside {
    color: white;
    padding: 30px;
    padding-left: 1em;
    padding-right: 1em;
    background: linear-gradient(to bottom, rgb(10, 68, 156), rgb(1, 28, 88));
    width: 35%;
    border-radius: 0 5px 5px 0;
  }

  aside > * {
    padding: 0;
    margin: 0;
    font-size: 1.7em;
  }

  aside h3 {
    margin-top: 30px;
  }

  aside h3:first-of-type {
    padding-top: 0;
  }

  aside p {
    font-size: 1.4em;
  }

  aside ul {
    font-size: 1.4em;
    margin-left: 50px;
  }

  aside h2:first-of-type {
    margin-top: 0;
  }

  h2 {
    margin-right: 2em;
    border-bottom: 5px solid white;
    margin-top: 30px;
    margin-bottom: 20px;
    font-size: 2em;
  }

  article {
    width: 65%;
    display: flex;
    flex-direction: column;
    padding-right: 1em;
    padding-left: 1em;
  }

  article h2 {
    border-bottom-color: rgb(10, 68, 156);
    margin-right: 0;
    color: rgb(10, 68, 156);
    font-size: 32px;
    margin-top: 20px;
  }

  main > div {
    padding: 0;
    display: flex;
  }

  section {
    font-size: 1.3em;
    color: rgb(5, 42, 53);
  }

  table {
    width: 100%;
    border-spacing: 0 15px;
  }

  .competences > div:last-of-type {
    display: flex;
  }

  .competences > div:first-of-type {
    display: flex;
    padding-left: 1.5em;
    padding-right: 11em;
    justify-content: space-between;
  }

  .competences li:first-of-type {
    padding-top: 0;
  }

  .competences li {
    padding-top: 20px;
  }

  .images {
    text-align: center;
    padding-top: 20px;
    width: 250px;
  }

  img {
    margin-bottom: 20px;
    width: 64px;
    height: 64px;
  }

  @media screen and (max-width: 900px ){
    :global(body) {
      display: initial;
      background-color: rgba(0, 0, 0, 0.1);
    }
  }
</style>
