# criando-site-html-javascript
 Multiverso Spider-Man: Criando um Site com HTML, CSS e JavaScript

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multiverso Spider-Man</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <h1>Bem-vindo ao Multiverso do Spider-Man</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#heroes">Heróis</a></li>
                <li><a href="#contact">Contato</a></li>
            </ul>
        </nav>
    </header>
    <section id="home" class="home">
        <h2>O que é o Multiverso?</h2>
        <p>O Multiverso é um conceito fascinante onde múltiplas realidades coexistem. Explore diferentes versões do Spider-Man!</p>
    </section>
    <section id="heroes" class="heroes">
        <h2>Heróis do Multiverso</h2>
        <div class="heroes-container">
            <div class="hero-card">
                <h3>Peter Parker</h3>
                <img src="path/to/peter-parker.jpg" alt="Peter Parker">
                <p>O Spider-Man original, conhecido por seu senso de responsabilidade e bravura.</p>
            </div>
            <div class="hero-card">
                <h3>Miles Morales</h3>
                <img src="path/to/miles-morales.jpg" alt="Miles Morales">
                <p>Um jovem herói que traz uma nova perspectiva ao legado do Spider-Man.</p>
            </div>
            <div class="hero-card">
                <h3>Gwen Stacy</h3>
                <img src="path/to/gwen-stacy.jpg" alt="Gwen Stacy">
                <p>Conhecida como Spider-Gwen, ela luta por justiça em seu próprio universo.</p>
            </div>
        </div>
    </section>
    <section id="contact" class="contact">
        <h2>Contato</h2>
        <form>
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Mensagem:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>
    <footer class="footer">
        <p>&copy; 2024 Multiverso Spider-Man. Todos os direitos reservados.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

.header {
    background-color: #000;
    color: #fff;
    padding: 20px;
    text-align: center;
}

.header h1 {
    margin: 0;
}

.header nav ul {
    list-style: none;
    padding: 0;
}

.header nav ul li {
    display: inline;
    margin: 0 10px;
}

.header nav ul li a {
    color: #fff;
    text-decoration: none;
}

.home, .heroes, .contact {
    padding: 50px 20px;
    text-align: center;
}

.heroes-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.hero-card {
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px;
    width: 200px;
    text-align: center;
}

.hero-card img {
    max-width: 100%;
    height: auto;
    border-radius: 5px;
}

.contact form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.contact form input, .contact form textarea {
    width: 100%;
    max-width: 500px;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact form button {
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    background-color: #000;
    color: #fff;
    cursor: pointer;
}

.contact form button:hover {
    background-color: #444;
}

.footer {
    background-color: #000;
    color: #fff;
    padding: 20px;
    text-align: center;
}
document.addEventListener('DOMContentLoaded', () => {
    const form = document.querySelector('form');

    form.addEventListener('submit', (e) => {
        e.preventDefault();
        alert('Formulário enviado com sucesso!');
    });
});
