<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Services Informatiques</title>
    <link rel="stylesheet" href="/* Réinitialisation de base */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
}

/* Bannière */
.banniere {
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(to right, #333, #555);
    padding: 20px;
    color: white;
}

.logo img {
    max-width: 300px;
    margin-right: 80px;
}

.titre h1 {
    margin: 0;
    font-size: 24px;
}

.titre p {
    margin: 5px 0 0;
    font-size: 14px;
}

/* Menu principal */
.menu {
    list-style: none;
    padding: 0;
    background: #f00d8a;
    display: flex;
    justify-content: center;
}

.menu li {
    position: relative;
}

.menu a {
    display: block;
    padding: 15px;
    color: white;
    text-decoration: none;
}

.menu a:hover {
    background: #555;
}

/* Sous-menus */
.submenu {
    display: none;
    position: absolute;
    background: #444;
    list-style: none;
    padding: 0;
    min-width: 200px;
    top: 100%;
    left: 0;
}

.submenu li {
    width: 100%;
}

.submenu a {
    padding: 10px;
    display: block;
    text-align: left;
}

.submenu a:hover {
    background: #666;
}

.dropdown:hover .submenu {
    display: block;
}

/* Carrousel */
.carousel {
    width: 100%;
    overflow: hidden;
    position: relative;
    max-width: 800px;
    margin: 20px auto;
}

.slider {
    display: flex;
    width: 300%;
    animation: slide 25s infinite;
}

.slide {
    width: 100%;
    flex: 1;
}

.slide img {
    width: 100%;
    height: auto;
}

/* Animation */
@keyframes slide {
    0% { transform: translateX(0); }
    33% { transform: translateX(-100%); }
    66% { transform: translateX(-200%); }
    100% { transform: translateX(0); }
}

/* Contenu principal */
.container {
    display: flex;
    max-width: 1200px;
    margin: auto;
    padding: 20px;
    gap: 20px;
}

/* Menu droit */
.menu-droit {
    flex: 1;
    background: #f4f4f4;
    padding: 20px;
    border-left: 2px solid #ddd;
}

.menu-droit h3 {
    color: #333;
}

.menu-droit ul {
    list-style: none;
    padding: 0;
}

.menu-droit ul li {
    margin: 5px 0;
}

.menu-droit ul li a {
    text-decoration: none;
    color: #007BFF;
}

.menu-droit ul li a:hover {
    text-decoration: underline;
}

.menu-droit p {
    font-size: 14px;
    color: #555;
}
/* 4 phases de la page d'accueil */
.phases {
    display: flex;
    justify-content: space-around;
    padding: 20px;
}

.phase {
    width: 22%;
    text-align: center;
}

.phase img {
    width: 100%;
    border-radius: 5px;
}

/* Correction du carrousel */
.carousel {
    position: relative;
    z-index: 0;
}

.menu {
    position: relative;
    z-index: 1;
}

/* Panneau à onglets */
.formulaires {
    max-width: 600px;
    margin: auto;
}

.tabs {
    display: flex;
    justify-content: space-around;
    background: #333;
    color: rgb(220, 15, 110);
    padding: 10px;
}

.tabs label {
    cursor: pointer;
    padding: 10px;
}

.contenu-form {
    background: #f4f4f4;
    padding: 20px;
    border-radius: 5px;
}

.formulaire {
    display: none;
}

#client:checked ~ .contenu-form #form-client,
#fournisseur:checked ~ .contenu-form #form-fournisseur,
#partenaire:checked ~ .contenu-form #form-partenaire {
    display: block;
}

input[type="radio"] {
    display: none;
}

/* Pied de page */
footer {
    background: #ed1283;
    color: white;
    padding: 10px;
    margin-top: 20px;
}">
</head>
<body>

    <!-- Bannière avec logo -->
    <header class="banniere">
        <div class="logo">
            <img src="IMG-20250317-WA0001.jpg" alt="Logo de l'entreprise">
        </div>
        <div class="titre">
            <h1>Services Informatiques</h1>
            <p>Votre partenaire technologique de confiance</p>
        </div>
    </header>

    <!-- Menu principal -->
    <nav>
        <ul class="menu">
            <li><a href="#">Accueil</a></li>
            <li class="dropdown">
                <a href="#">Présentation</a>
                <ul class="submenu">
                    <li><a href="historique.html">Historique</a></li>
                    <li><a href="Mission.html">Mission</a></li>
                    <li><a href="Equipe.html">Équipe</a></li>
                </ul>
            </li>
            <li class="dropdown">
                <a href="#">Prestations</a>
                <ul class="submenu">
                    <li><a href="réseaux informatique.html">Réseaux informatiques</a></li>
                    <li><a href="Télécommunication.html">Télécommunications </a></li>
                    <li><a href="genie logiciel.html">Génie Logiciel</a></li>
                    <li><a href="intélligence économique.html">Intelligence économique</a></li>
                    <li><a href="technologie-internet.html">Technologie internet</a></li>
                    <li><a href="sécurité des SI.html">Sécurité des SI</a></li>
                </ul>
            </li>
            <li class="dropdown">
                <a href="#">Formations</a>
                <ul class="submenu">
                    <li><a href="certification.html">Certifications</a></li>
                    <li><a href="Séminaire.html">Séminaires</a></li>
                    <li><a href="conférence.html">Conférences</a></li>
                    <li><a href="Atéliers.html">Ateliers</a></li>
                </ul>
            </li>
            <li class="dropdown">
                <a href="#">Partenaires</a>
                <ul class="submenu">
                <li><a href="nationaux.html">Nationaux </a></li>
                <li><a href="internationaux.html"> Inter nations </a></li>
            </ul>
        </li>
        <li class="dropdown">
            <a href="">Support</a>
            <ul class="submenu">
                <li><a href="assistance.html">Assistance </a></li>
                <li><a href="Téléchargement.html"> téléchargement</a></li>
            </ul>
        </li>
            <li><a href="Contact.html">Contacts</a></li>
        </ul>
    </nav>

    <!-- Carrousel d'images -->
    <section class="carousel">
        <div class="slider">
            <div class="slide"><img src="slide1.jpg" alt="Slide 1"></div>
            
            <div class="slide"><img src="slide2.jpg" alt="Slide 2"></div>
            
            <div class="slide"><img src="slide3.jpg" alt="Slide 3"></div>
           
            <div class="slide"><img src="slide1.jpg" alt="Slide 1"></div>
            
            <div class="slide"><img src="slide2.jpg" alt="Slide 2"></div>
            
            <div class="slide"><img src="slide3.jpg" alt="Slide 3"></div>
          
            <div class="slide"><img src="slide1.jpg" alt="Slide 1"></div>
            
            <div class="slide"><img src="slide2.jpg" alt="Slide 2"></div>
            
            <div class="slide"><img src="slide3.jpg" alt="Slide 3"></div>
           
            <div class="slide"><img src="slide1.jpg" alt="Slide 1"></div>
            
            <div class="slide"><img src="slide2.jpg" alt="Slide 2"></div>
            
            <div class="slide"><img src="slide3.jpg" alt="Slide 3"></div>
        </div>
    </section>

    <!-- Contenu principal et menu droit -->
    <div class="container">
        <main class="contenu">
            <h2>À PROPOS DE SERVICE INFORMATIQUE</h2>
            <p>Nous fournissons des solutions informatiques de pointe pour optimiser votre entreprise.</p>
            <img src="c:\Users\1030\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\3F20872CFEE4278DBA7B3C0D18D370F8\WhatsApp Image 2025-04-01 à 21.15.55_08b39128.jpg" alt="Service 2">
        </main>

        <aside class="menu-droit">
            <h3>À propos</h3>
            <p>Nous sommes une entreprise spécialisée dans les services informatiques, offrant des solutions adaptées aux besoins des entreprises.</p>

            <h3>Liens Utiles</h3>
            <ul>
                <li><a href="documentation.html">Documentation</a></li>
                <li><a href="support technique.html">Support technique</a></li>
                <li><a href="FAQ.html">FAQ</a></li>
                <li><a href="contactez-nous.html">Contactez-nous</a></li>
            </ul>

            <h3>Actualités</h3>
            <p>🔹 Nouveau partenariat avec XYZ Corp.<br>🔹 Prochaine formation sur la cybersécurité - Inscrivez-vous !</p>
        </aside>
    </div>

    <!-- 4 phases de la page d'accueil -->
    <section class="phases">
        <div class="phase">
            <img src="sous1.jpg" alt="Service 1">
            <h>🔹 Conseil en transformation digitale</h>
        <p>Un projet de transformation digitale nécessite du temps et c’est un réel défi pour les entreprises souhaitant passer par là.

            Pour assurer la réussite d’un projet d’une telle envergure, la communication est la clé !
            
            Impossible d’avancer si vous et vos collaborateurs ne vous laissez pas le temps d’échanger sur vos visions, réticences et questions.</p>
        </div>
        <div class="phase">
            <img src="sous2.jpg" alt="Service 2">
            <h>🔹 Sécurité des systèmes d'information </h>
            <p> La sécurité de l'information n'est confinée ni aux systèmes informatiques, ni à l'information dans sa forme numérique ou électronique. Au contraire, elle s'applique à tous les aspects de la sûreté, la garantie, et la protection d'une donnée ou d'une information, quelle que soit sa forme.</p>
        </div>
        <div class="phase">
            <img src="sous3.jpg" alt="Service 3">
            <h>🔹 Développement de logiciels sur mesure</h>
        <p>L’un de ses enjeux majeurs est de trouver sur le marché des outils qui lui soient parfaitement adaptés, non des solutions standards faites pour le plus grand nombre et que, bien souvent, elle choisit par défaut.</p>
        </div>
        <div class="phase">
            <img src="sous4.jpg" alt="Service 4">
            <h>🔹 Maintenance et support technique</h>
        <p>Nous effectuons des opérations de maintenance sur votre parc informatique et garantissons sa robustesse dans le temps. Pour se faire, nous opérons au travers de deux modèles : la maintenance proactive, la plus anticipative possible, mais est souvent postérieure à l’incident. La maintenance préventive, qui permet grâce à la solution de monitoring Centreon, la prévention des ruptures de service.</p>
        </div>
    </section>

    <!-- Panneau à onglets pour les formulaires -->
    <section class="formulaires">
        <input type="radio" id="client" name="tab" checked>
        <input type="radio" id="fournisseur" name="tab">
        <input type="radio" id="partenaire" name="tab">

        <div class="tabs">
            <label for="client">Client</label>
            <label for="fournisseur">Fournisseur</label>
            <label for="partenaire">Partenaire</label>
        </div>

        <div class="contenu-form">
            <div class="formulaire" id="form-client">
                <h3>Enregistrement Client</h3>
                <form>
                    <input type="text" placeholder="Nom">
                    <input type="email" placeholder="Email">
                    <input type="tel" placeholder="Téléphone">
                    
                    <button type="submit">S'inscrire</button>
                </form>
            </div>

            <div class="formulaire" id="form-fournisseur">
                <h3>Enregistrement Fournisseur</h3>
                <form>
                    <input type="text" placeholder="Entreprise">
                    <input type="email" placeholder="Email">
                    <input type="tel" placeholder="Téléphone">
                    
                    <button type="submit">S'inscrire</button>
                </form>
            </div>

            <div class="formulaire" id="form-partenaire">
                <h3>Enregistrement Partenaire</h3>
                <form>
                    <input type="text" placeholder="Nom">
                    <input type="email" placeholder="Email">
                    <input type="tel" placeholder="Téléphone">
                    
                    <button type="submit">S'inscrire</button>
                </form>
            </div>
        </div>
    </section>

    <footer>
        <p>Services Informatiques KADY</p>
    </footer>

</body>
</html>
