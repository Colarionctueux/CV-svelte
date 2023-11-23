<main>
  <h1>NICOLAS ECKMAN</h1>
  <p>
    Actuellement étudiant en BUT informatique<br />
    à L’IUT A de Lille, je suis passionné d’informatique<br />
    et aime apprendre dans tous les domaines.
  </p>
  <div>
    <aside>
      <h2>PROFIL</h2>
      <h3>Téléphone</h3>
      <p>07 71 85 23 08</p>
      <h3>E-mail</h3>
      <p>nicolas.eckmanpro@gmail.com</p>
      <h3>Date de naissance</h3>
      <p>13 mars 2004</p>
      <h3>Lien github</h3>
      <a href="https://github.com/Colarionctueux">Colarionctueux</a>
      <h2>QUALITÉS</h2>
      <ul>
        <li>Serieux</li>
        <li>Travail en équipe</li>
        <li>Adaptation</li>
        <li>Communication</li>
      </ul>
      <h2>LANGUES</h2>
      <ul>
        <li>Français - natif</li>
        <li>Anglais - B2</li>
        <li>Allemand - bases</li>
      </ul>
    </aside>
    <article>
      <section>
        <h2>FORMATION</h2>
        <table>
          <tbody>
            <tr>
              <th>Actuellement</th>
              <td><b>BUT Informatique</b><br />IUT de Lille</td>
            </tr>
            <tr>
              <th>2022</th>
              <td
                ><b>Baccalauréat<br />Spécialités Maths - NSI</b><br />Lycée
                Raymond Queneau</td
              >
            </tr>
          </tbody>
        </table>
      </section>
      <section class="competences">
        <h2>COMPÉTENCES</h2>
        <div>
          <b>Développement</b>
          <b>Projets</b>
        </div>
        <div transition:blur>
          <div class="images">
            <img src="/java.svg" alt="logo java" />
            <img src="/bash.svg" alt="logo bash" />
            <img src="/html.svg" alt="logo html" />
            <img src="/css.svg" alt="logo css" />
            <img src="/c.svg" alt="logo c" />
            <img src="/psql.svg" alt="logo psql" />
          </div>
          <ul>
            <li>Jeu - Méthode agile, Java</li>
            <li>SQL - Gestion base de donnée, Requêtage</li>
            <li>IHM - Application d'échange linguistique</li>
            <li>HTML - Site d'aide au covoiturage</li>
          </ul>
        </div>
      </section>
      <section>
        <h2>EXPÉRIENCE</h2>
        <table>
          <tbody>
            <tr>
              <th>2022</th>
              <td><b>Agent d'accueil</b><br />Basic-Fit</td>
            </tr>
            <tr>
              <th>2019</th>
              <td><b>Stage d'observation</b><br />Sogeti - Capgemini</td>
            </tr>
          </tbody>
        </table>
      </section>
    </article>
  </div>
</main>

<style>
  :global(*) {
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  }

  :global(body) {
    display: flex;
    margin: 0;
    justify-content: center;
    padding: 30px;
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
</style>
