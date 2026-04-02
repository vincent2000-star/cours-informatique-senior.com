<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Plateforme Informatique</title>

<style>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: #f5f7ff;
}

/* NAV */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 30px;
    background: #007BFF;
    color: white;
}

nav button {
    margin-left: 10px;
    background: white;
    color: #007BFF;
    border-radius: 20px;
    padding: 8px 15px;
}

/* HERO */
.hero {
    text-align: center;
    padding: 80px 20px;
    background: linear-gradient(135deg, #007BFF, #00c6ff);
    color: white;
}

/* CONTAINER */
.container {
    max-width: 1100px;
    margin: auto;
    padding: 30px;
}

/* CARDS */
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    gap: 20px;
}

.card {
    background: white;
    padding: 20px;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    cursor: pointer;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-5px);
}

/* PROGRESS */
.progress {
    background: #ddd;
    border-radius: 20px;
    overflow: hidden;
    margin-top: 10px;
}

.progress-bar {
    height: 10px;
    width: 30%;
    background: #007BFF;
}

/* MODAL */
.modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.6);
    display: none;
    justify-content: center;
    align-items: center;
}

.modal-content {
    background: white;
    padding: 30px;
    border-radius: 10px;
    max-width: 500px;
}

/* FAQ */
.faq-item {
    background: white;
    padding: 15px;
    margin: 10px 0;
    cursor: pointer;
    border-radius: 10px;
}

.answer {
    display: none;
    margin-top: 10px;
}

/* FORM */
form {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

input, textarea {
    padding: 10px;
    border-radius: 5px;
    border: 1px solid #ccc;
}

/* BUTTON */
button {
    padding: 10px;
    border: none;
    background: #007BFF;
    color: white;
    cursor: pointer;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 20px;
    background: #111;
    color: #aaa;
}
</style>
</head>

<body>

<nav>
    <div>🎓 Informatique Facile</div>
    <div>
        <button onclick="login()">Connexion</button>
        <button onclick="showPricing()">Tarifs</button>
    </div>
</nav>

<div class="hero">
    <h1>Apprenez l'informatique</h1>
    <p>Formations professionnelles accessibles à tous</p>
</div>

<div class="container">

<h2>📚 Cours disponibles</h2>

<div class="cards">
    <div class="card" onclick="openCourse('ordinateur')">
        <h3>💻 Débuter ordinateur</h3>
        <p>Formation complète pour débutants</p>
        <div class="progress"><div class="progress-bar"></div></div>
    </div>

    <div class="card" onclick="openCourse('internet')">
        <h3>🌐 Internet</h3>
        <p>Naviguer en toute sécurité</p>
    </div>

    <div class="card" onclick="openCourse('email')">
        <h3>📧 Email</h3>
        <p>Maîtriser la communication en ligne</p>
    </div>
</div>

<h2>❓ FAQ</h2>

<div class="faq-item" onclick="toggleFaq(this)">
Comment apprendre rapidement ?
<div class="answer">Pratiquez régulièrement et suivez les cours dans l’ordre.</div>
</div>

<div class="faq-item" onclick="toggleFaq(this)">
Est-ce payant ?
<div class="answer">Oui, nos formations sont accessibles via abonnement mensuel.</div>
</div>

<h2>📩 Contact</h2>

<form onsubmit="sendMessage(event)">
<input type="text" placeholder="Nom" required>
<input type="email" placeholder="Email" required>
<textarea placeholder="Message"></textarea>
<button>Envoyer</button>
</form>

</div>

<footer>
© 2026 Plateforme Informatique
</footer>

<!-- MODAL -->
<div class="modal" id="modal">
    <div class="modal-content" id="modalContent"></div>
</div>

<script>

function login(){
    alert("Connexion bientôt disponible !");
}

function showPricing(){
    document.getElementById("modalContent").innerHTML = `
        <h2>Nos tarifs</h2>
        <p><strong>Abonnement mensuel :</strong> 9,99€</p>
        <p>Accès complet à tous les cours</p>
        <button onclick="alert('Paiement bientôt disponible')">S'abonner</button>
    `;
    document.getElementById("modal").style.display = "flex";
}

function openCourse(course){
    let content = "";

    if(course === "ordinateur"){
        content = "<h2>Débuter ordinateur</h2><p>Allumer un ordinateur, utiliser la souris et le clavier.</p>";
    }
    if(course === "internet"){
        content = "<h2>Internet</h2><p>Utiliser un navigateur et faire des recherches.</p>";
    }
    if(course === "email"){
        content = "<h2>Email</h2><p>Créer et envoyer des emails facilement.</p>";
    }

    document.getElementById("modalContent").innerHTML = content;
    document.getElementById("modal").style.display = "flex";
}

document.getElementById("modal").onclick = function(){
    this.style.display = "none";
}

function toggleFaq(el){
    let ans = el.querySelector(".answer");
    ans.style.display = ans.style.display === "block" ? "none" : "block";
}

function sendMessage(e){
    e.preventDefault();
    alert("Message envoyé !");
}

</script>

</body>
</html>
