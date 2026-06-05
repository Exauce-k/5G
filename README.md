<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>5G Business</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #0a0a0a;
    color: white;
}

/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    padding: 20px;
    background: black;
    border-bottom: 2px solid gold;
}

header h1 {
    color: gold;
}

nav a {
    margin: 0 10px;
    color: white;
    text-decoration: none;
}

nav a:hover {
    color: gold;
}

/* HERO */
.hero {
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: linear-gradient(black, #111);
    text-align: center;
}

.hero h2 {
    font-size: 45px;
    color: gold;
    animation: fadeIn 2s;
}

.hero p {
    margin: 15px 0;
}

.hero button {
    padding: 12px 25px;
    background: gold;
    border: none;
    cursor: pointer;
    font-weight: bold;
}

.hero button:hover {
    background: orange;
}

/* SECTIONS */
.section {
    padding: 50px 20px;
    text-align: center;
}

.cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    background: #111;
    margin: 15px;
    padding: 25px;
    width: 260px;
    border-radius: 10px;
    border: 1px solid gold;
    transition: 0.3s;
}

.card:hover {
    transform: scale(1.05);
    box-shadow: 0 0 15px gold;
}

.card h3 {
    color: gold;
}

/* WHATSAPP BUTTON */
.whatsapp {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #25D366;
    padding: 15px;
    border-radius: 50%;
    text-align: center;
    font-size: 20px;
}

.whatsapp a {
    color: white;
    text-decoration: none;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 20px;
    background: black;
    border-top: 2px solid gold;
}

/* ANIMATION */
@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}

/* RESPONSIVE */
@media(max-width: 600px) {
    .hero h2 {
        font-size: 30px;
    }
}
</style>

</head>

<body>

<header>
    <h1>Litework</h1>
    <nav>
        <a href="#">Accueil</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <h2>Bienvenue dans Litework</h2>
    <p>Design • Musique • Business</p>
    <button onclick="scrollToServices()">Découvrir</button>
</section>

<section class="section" id="services">
    <h2>Nos Services</h2>

    <div class="cards">
        <div class="card">
            <h3>5G DESIGN</h3>
            <p>Logos, affiches, branding professionnel.</p>
        </div>

        <div class="card">
            <h3>5G MUSIC</h3>
            <p>Production et promotion musicale.</p>
        </div>

        <div class="card">
            <h3>5G SHOP</h3>
            <p>Vente de produits alimentaires à Kinshasa.</p>
        </div>
    </div>
</section>

<section class="section">
    <h2>À propos</h2>
    <p>
        5G Business est une vision entrepreneuriale créée par Exauce Kaboto,
        visant à construire une marque forte et innovante.
    </p>
</section>

<section class="section" id="contact">
    <h2>Contact</h2>
    <p>WhatsApp : +243 987556477</p>
      <p>WhatsApp : +243 851643612</p>
      <p>WhatsApp : +243 808731409</p>
    
    <p>Email : exaucekaboto47@gmail.com.com</p>
</section>

<footer>
    <p>© 2026 WorkLite</p>
</footer>

<!-- WHATSAPP FLOAT -->
<div class="whatsapp">
    <a href="https://wa.me/243987556477" target="_blank">💬</a>
</div>

<script>
function scrollToServices() {
    document.getElementById("services").scrollIntoView({ behavior: "smooth" });
}
</script>

</body>
</html>
