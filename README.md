<!doctype html>
<html lang="en"> 
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Label Tlv</title> 
 </head> 
 <body> <!-- Section de Connexion --> 
  <section id="connexion"> 
   <h2>Connexion</h2> 
   <form action="/connexion" method="post"> <label for="username">Nom d'utilisateur :</label> 
    <input type="text" id="username" name="username" required> <label for="password">Mot de passe :</label> 
    <input type="password" id="password" name="password" required> <button type="submit">Se Connecter</button> 
   </form> 
  </section> <!-- Formulaire d'Inscription pour les Artistes --> 
  <section id="inscriptionArtiste"> 
   <h2>Inscription Artiste</h2> 
   <form action="/inscription" method="post"> <label for="artistName">Nom d'Artiste :</label> 
    <input type="text" id="artistName" name="artistName" required> <label for="email">Adresse E-mail :</label> 
    <input type="email" id="email" name="email" required> <label for="password">Mot de passe :</label> 
    <input type="password" id="password" name="password" required> <label for="confirmPassword">Confirmer le Mot de passe :</label> 
    <input type="password" id="confirmPassword" name="confirmPassword" required> <button type="submit">S'Inscrire</button> 
   </form> 
  </section> <!-- Tarification avec Ventes d'Albums --> 
  <section id="tarification"> 
   <h2>Tarification</h2> 
   <p>Consultez nos offres spéciales pour les albums et les EP :</p> 
   <div class="album"> 
    <h3>Nom de l'Album</h3> 
    <p>Prix :</p> <button onclick="acheterAlbum()">Acheter</button> 
    <div id="lienTelechargement" style="display: none;"> <a href="/telechargement/nom-de-l-album.zip" download>Télécharger l'Album</a> 
    </div> 
   </div> 
  </section> <!-- Coordonnées --> 
  <section id="coordonnees"> 
   <h2>Nos Coordonnées</h2> 
   <address> <strong>Votre Nom Georges/ Label Tlv</strong><br> Adresse physique, Le Havre, France <br> Numéro de téléphone : +33 6 68 16 11 83<br> Adresse e-mail: tlv76610@outlook.fr </address> 
  </section> <!-- Script pour changer la couleur du fond --> 
  <script>
        function acheterAlbum() {
            document.getElementById('lienTelechargement').style.display = 'block';
        }
    </script> 
 </body>
</html>
/* Reset CSS pour normaliser les styles entre les navigateurs */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Style de base pour le corps de la page */
body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Style du conteneur principal */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

/* Style du menu de navigation */
nav {
    background-color: #222;
    padding: 10px 0;
}

nav ul {
    list-style: none;
}

nav li {
    display: inline-block;
    margin-right: 20px;
}

nav a {
    text-decoration: none;
    color: #fff;
    font-weight: bold;
}

/* Style de l'en-tête */
header {
    text-align: center;
    padding: 50px 0;
}

header h1 {
    font-size: 2.5em;
    color: #333;
}

/* Style des sections principales */
section {
    margin-bottom: 40px;
}

/* Style du pied de page */
footer {
    background-color: #222;
    color: #fff;
    text-align: center;
    padding: 20px 0;
}

/* Style des liens dans le pied de page */
footer a {
    color: #fff;
    text-decoration: none;
    margin: 0 10px;
}

/* Style des boutons */
.button {
    display: inline-block;
    padding: 10px 20px;
    font-size: 1em;
    text-align: center;
    text-decoration: none;
    background-color: #3498db;
    color: #fff;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.button:hover {
    background-color: #2980b9;
}
