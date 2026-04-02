<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apprendre l'Informatique</title>

    <style>
    <header>
    <h1 style="display:none;">cours-informatique-senior.com</h1>
    <h1>Bienvenue sur le site d'apprentissage informatique</h1>
    <p>Apprenez à votre rythme, simplement et efficacement</p>
</header>

👉 Ça masque l’ancien titre
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: linear-gradient(to right, #eef, #dde7ff);
            color: #333;
        }

        header {
            text-align: center;
            padding: 30px 20px 10px;
        }

        nav {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            background: #007BFF;
            padding: 10px;
            border-radius: 0 0 10px 10px;
        }

        nav a {
            margin: 10px;
            text-decoration: none;
            font-size: 18px;
            color: white;
            font-weight: bold;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.7;
        }

        section {
            max-width: 800px;
            margin: 30px auto;
            padding: 25px;
            border-radius: 10px;
            background: #fff;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        h1, h2 {
            text-align: center;
        }

        button {
            padding: 12px 25px;
            font-size: 16px;
            background: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        button:hover {
            background: #0056b3;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        input, textarea {
            padding: 10px;
            font-size: 16px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        footer {
            text-align: center;
            padding: 20px;
            font-size: 14px;
            color: #666;
        }
    </style>
</head>

<body>

<header>
    <h1>Bienvenue sur le site d'apprentissage informatique</h1>
    <p>Apprenez à votre rythme, simplement et efficacement</p>
</header>

<nav>
    <a href="#accueil">Accueil</a>
    <a href="#cours">Cours</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</nav>

<section id="accueil">
    <h2>Accueil</h2>
    <p>Ce site vous accompagne pour apprendre l'informatique facilement, quel que soit votre niveau.</p>
</section>

<section id="cours">
    <h2>Cours</h2>
    <p>Découvrez des cours progressifs : utiliser un ordinateur, envoyer un email, naviguer sur Internet, et bien plus.</p>
    <button onclick="alert('Les cours détaillés arrivent bientôt !')">Voir les cours</button>
</section>

<section id="faq">
    <h2>FAQ</h2>
    <p>Consultez les réponses aux questions les plus fréquentes sur l'utilisation de l'informatique.</p>
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
    © 2026 - Apprentissage informatique
</footer>

</body>
</html>
