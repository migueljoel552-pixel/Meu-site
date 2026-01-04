<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Joel Sebastião | Criação de Sites Profissionais</title>

    <meta name="description" content="Joel Sebastião cria sites profissionais, designs e soluções digitais para negócios em Angola.">

    <style>
        :root {
            --primary: #667eea;
            --secondary: #764ba2;
            --dark: #333;
            --light: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            color: var(--dark);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav {
            max-width: 1200px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 2rem;
        }

        .logo {
            font-weight: bold;
            font-size: 1.4rem;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
        }

        section {
            max-width: 1200px;
            margin: auto;
            padding: 5rem 2rem;
        }

        .hero {
            margin-top: 80px;
            text-align: center;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 7rem 2rem;
        }

        .hero h1 {
            font-size: 2.5rem;
        }

        .hero p {
            margin: 1rem 0 2rem;
            font-size: 1.2rem;
        }

        .btn {
            background: white;
            color: var(--primary);
            padding: 1rem 2rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            color: var(--primary);
            margin-bottom: 3rem;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            align-items: center;
        }

        .profile-pic {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 6rem;
            color: white;
            margin: auto;
        }

        .services {
            background: var(--light);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
        }

        .service-card h3 {
            color: var(--primary);
            margin: 1rem 0;
        }

        .contact-form {
            max-width: 500px;
            margin: auto;
        }

        input, textarea {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        button {
            width: 100%;
            padding: 1rem;
            border: none;
            border-radius: 30px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            font-weight: bold;
        }

        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem;
        }

        /* WhatsApp */
        .whatsapp {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #25d366;
            color: white;
            padding: 1rem;
            border-radius: 50%;
            font-size: 1.5rem;
            text-decoration: none;
        }

        @media(max-width:768px){
            .about-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>

<header>
    <nav>
        <div class="logo">Joel Sebastião</div>
        <ul class="nav-links">
            <li><a href="#inicio">Início</a></li>
            <li><a href="#sobre">Sobre</a></li>
            <li><a href="#servicos">Serviços</a></li>
            <li><a href="#contato">Contato</a></li>
        </ul>
    </nav>
</header>

<section id="inicio" class="hero">
    <h1>Criação de Sites Profissionais</h1>
    <p>Ajudo negócios e pessoas a crescerem na internet</p>
    <a href="#contato" class="btn">Fale Comigo</a>
</section>

<section id="sobre">
    <h2 class="section-title">Sobre Mim</h2>
    <div class="about-content">
        <div>
            <p>Sou Joel Sebastião, programador iniciante focado em criação de sites modernos, simples e eficazes para pequenos negócios.</p>
            <ul>
                <li>✔ HTML & CSS</li>
                <li>✔ Design com Canva</li>
                <li>✔ Edição com CapCut</li>
            </ul>
        </div>
        <div class="profile-pic">👤</div>
    </div>
</section>

<section id="servicos" class="services">
    <h2 class="section-title">Serviços</h2>
    <div class="services-grid">
        <div class="service-card">
            <h3>Design Gráfico</h3>
            <p>Logótipos, cartazes e posts.</p>
        </div>
        <div class="service-card">
            <h3>Criação de Sites</h3>
            <p>Sites profissionais e responsivos.</p>
        </div>
        <div class="service-card">
            <h3>Páginas HTML</h3>
            <p>Sites simples para negócios locais.</p>
        </div>
    </div>
</section>

<section id="contato">
    <h2 class="section-title">Contato</h2>
    <form class="contact-form" onsubmit="enviar(event)">
        <input type="text" placeholder="Seu nome" required>
        <input type="email" placeholder="Seu email" required>
        <textarea placeholder="Sua mensagem" required></textarea>
        <button>Enviar</button>
    </form>
</section>

<footer>
    <p>© 2025 Joel Sebastião</p>
    <p>WhatsApp: +244 942 424 066</p>
</footer>

<a class="whatsapp" href="https://wa.me/244942424066" target="_blank">💬</a>

<script>
    function enviar(e){
        e.preventDefault();
        alert("Mensagem enviada com sucesso!");
        e.target.reset();
    }
</script>

</body>
</html>
