<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Apprendre l'informatique facilement</title>

<style>
    body {
        font-family: 'Segoe UI', Arial, sans-serif;
        margin: 0;
        background: linear-gradient(to right, #eef2ff, #dfe9ff);
        color: #333;
    }

    header {
        text-align: center;
        padding: 50px 20px;
        background: linear-gradient(135deg, #007BFF, #0056b3);
        color: white;
    }

    header h1 {
        margin-bottom: 10px;
        font-size: 32px;
    }

    nav {
        position: sticky;
        top: 0;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        background: #007BFF;
        padding: 10px;
        z-index: 1000;
    }

    nav a {
        margin: 10px;
        text-decoration: none;
        font-size: 18px;
        color: white;
        font-weight: bold;
        padding: 8px 15px;
        border-radius: 5px;
        transition: 0.3s;
    }

    nav a:hover {
        background: rgba(255,255,255,0.2);
    }

    section {
        max-width: 900px;
        margin: 30px auto;
        padding: 30px;
        border-radius: 12px;
        background: white;
        box-shadow: 0 6px 20px rgba(0,0,0,0.1);
        animation: fadeIn 0.8s ease;
    }

    h2 {
        text-align: center;
        margin-bottom: 20px;
        color: #007BFF;
    }

    button {
        padding: 12px 25px;
        font-size: 16px;
        background: linear-gradient(135deg, #007BFF, #0056b3);
        color: white;
        border: none;
        border-radius: 25px;
        cursor: pointer;
        transition: 0.3s;
    }

    button:hover {
        transform: scale(1.05);
    }

    form {
        display: flex;
        flex-direction: column;
        gap: 12px;
    }

    input, textarea {
        padding: 12px;
        font-size: 16px;
        border-radius: 8px;
        border: 1px solid #ccc;
        transition: 0.3s;
    }

    input:focus, textarea:focus {
        border-color: #007BFF;
        outline: none;
    }

    footer {
        text-align: center;
        padding: 25px;
        font-size: 14px;
        background: #222;
        color: #aaa;
    }

    footer p {
        margin: 5px 0;
    }

    @keyframes fadeIn {
        from {opacity: 0; transform: translateY(20px);}
        to {opacity: 1; transform: translateY(0);}
    }

    @media (max-width: 600px) {
        header h1 {
            font-size: 24px;
        }

        nav a {
            font-size: 16px;
        }
    }
</style>
</head>

<body>

<header>
    <h1>Apprendre l'informatique simplement</h1>
    <p>Des cours clairs pour débutants et seniors</p>
</header>

<nav>
    <a href="#accueil">Accueil</a>
    <a href="#cours">Cours</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</nav>

<section id="accueil">
    <h2>Accueil</h2>
    <p>Bienvenue ! Ce site vous aide à apprendre l'informatique facilement, étape par étape, même si vous débutez totalement.</p>
</section>

<section id="cours">
    <h2>Cours</h2>
    <p>Apprenez à utiliser un ordinateur, envoyer des emails, naviguer sur Internet et bien plus encore.</p>
    <button onclick="alert('Les cours arrivent bientôt !')">Voir les cours</button>
</section>

<section id="faq">
    <h2>FAQ</h2>
    <p>Vous avez une question ? Consultez les réponses les plus fréquentes.</p>
</section>

<section id="contact">
    <h2>Contact</h2>
    <p>Une question ? Envoyez-nous un message :</p>
    <form>
        <input type="text" placeholder="Votre nom" required>
        <input type="email" placeholder="Votre email" required>
        <textarea placeholder="Votre message" rows="4" required></textarea>
        <button type="submit">Envoyer</button>
    </form>
</section>

<footer>
    <p>© 2026 - Apprentissage informatique</p>
    <p>Site éducatif pour débutants</p>
</footer>

</body>
</html>
