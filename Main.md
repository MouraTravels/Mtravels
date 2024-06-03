<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roteiros de Viagem</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #008cba;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #ddd;
            color: black;
        }
        .container {
            padding: 20px;
        }
        .hero {
            background-image: url('background.jpg');
            background-size: cover;
            color: white;
            padding: 100px 20px;
            text-align: center;
        }
        .cards {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .card {
            background-color: white;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            margin: 20px;
            max-width: 300px;
            text-align: center;
            transition: transform 0.2s;
        }
        .card:hover {
            transform: scale(1.05);
        }
        .card img {
            border-radius: 5px 5px 0 0;
            width: 100%;
        }
        .card h3 {
            color: #008cba;
            padding: 10px;
        }
        .card p {
            padding: 0 10px 10px;
        }
        .contact-form, .review-section, .custom-trip-form {
            background-color: white;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            margin: 20px 0;
            padding: 20px;
        }
        footer {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <h1>Roteiros de Viagem</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#roteiros">Roteiros</a>
        <a href="#custom">Roteiros Personalizados</a>
        <a href="#contact">Contacto</a>
        <a href="#reviews">Reviews</a>
    </nav>
    <div id="home" class="container hero">
        <h2>Descubra o Mundo com Nossos Roteiros</h2>
        <p>Escolha o roteiro perfeito para sua próxima aventura</p>
    </div>
    <div id="roteiros" class="container">
        <h2>Roteiros Disponíveis</h2>
        <div class="cards">
            <div class="card">
                <img src="trip1.jpg" alt="Trip 1">
                <h3>Roteiro 1</h3>
                <p>Descrição do Roteiro 1</p>
            </div>
            <div class="card">
                <img src="trip2.jpg" alt="Trip 2">
                <h3>Roteiro 2</h3>
                <p>Descrição do Roteiro 2</p>
            </div>
            <div class="card">
                <img src="trip3.jpg" alt="Trip 3">
                <h3>Roteiro 3</h3>
                <p>Descrição do Roteiro 3</p>
            </div>
        </div>
    </div>
    <div id="custom" class="container custom-trip-form">
        <h2>Crie Seu Roteiro Personalizado</h2>
        <form>
            <label for="dates">Datas Exatas:</label>
            <input type="date" id="dates" name="dates"><br><br>
            <label for="days">Número de Dias/Noites:</label>
            <input type="number" id="days" name="days" min="1"><br><br>
            <label for="location">Local:</label>
            <input type="text" id="location" name="location"><br><br>
            <label for="type">Tipo de Viagem:</label>
            <select id="type" name="type">
                <option value="leisure">Lazer</option>
                <option value="relax">Descanso</option>
                <option value="explore">Descobrir o País</option>
            </select><br><br>
            <label for="preferences">Preferências:</label><br>
            <input type="checkbox" id="beaches" name="preferences" value="beaches">
            <label for="beaches">Praias</label><br>
            <input type="checkbox" id="nature" name="preferences" value="nature">
            <label for="nature">Natureza</label><br>
            <input type="checkbox" id="museums" name="preferences" value="museums">
            <label for="museums">Museus</label><br>
            <input type="checkbox" id="historical" name="preferences" value="historical">
            <label for="historical">Parte Antiga da Cidade</label><br>
            <input type="checkbox" id="history" name="preferences" value="history">
            <label for="history">Coisas Históricas</label><br><br>
            <button type="submit">Enviar</button>
        </form>
    </div>
    <div id="contact" class="container contact-form">
        <h2>Contacto</h2>
        <form>
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name"><br><br>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email"><br><br>
            <label for="message">Mensagem:</label><br>
            <textarea id="message" name="message" rows="4" cols="50"></textarea><br><br>
            <button type="submit">Enviar</button>
        </form>
    </div>
    <div id="reviews" class="container review-section">
        <h2>Reviews</h2>
        <div class="review">
            <p><strong>João:</strong> Adorei o roteiro! Tudo estava perfeitamente organizado.</p>
        </div>
        <div class="review">
            <p><strong>Maria:</strong> Excelente experiência, recomendo a todos!</p>
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Roteiros de Viagem. Todos os direitos reservados.</p>
    </footer>
    <script>
        // Aqui você pode adicionar funcionalidades de chat e outras interações dinâmicas
        // Exemplo simples de alerta ao clicar no botão de enviar
        document.querySelector('button[type="submit"]').addEventListener('click', function(event) {
            event.preventDefault();
            alert('Formulário enviado!');
        });
    </script>
</body>
</html>
