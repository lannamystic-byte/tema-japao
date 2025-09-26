<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cultura Japonesa - Tradição e Modernidade</title>
    <style>
        /* Estilos gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
 .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
                /* Cabeçalho */
        header {
            background-color: #bc002d; /* Vermelho japonês */
            color: white;
            padding: 20px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
                .header-content {

display: flex;
            justify-content: space-between;
            align-items: center;
        }
                .logo {
            font-size: 2rem;
            font-weight: bold;
            display: flex;
            align-items: center;
        }
        
.logo span {
            margin-left: 10px;
        }
                nav ul {
            display: flex;
            list-style: none;
        }
        
nav ul li {
            margin-left: 20px;
        }
                nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
 nav ul li a:hover {
            color: #ffd700; /* Dourado */
        }
                /* Banner */
        .banner {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1528164344705-47542687000d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 500px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
        }
        
.banner-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
                .banner-content p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto;
        }
        
/* Seções */
        section {
            padding: 60px 0;
        }
                .section-title {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }
        
.section-title h2 {
            font-size: 2.5rem;
            color: #bc002d;
            display: inline-block;
            padding-bottom: 10px;
        }
                .section-title h2::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 3px;
            background-color: #bc002d;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }
        
/* Sobre */
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
                .about-text {
            flex: 1;
        }
        
.about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
.about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
                /* Tradições */
        .traditions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
.tradition-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
                .tradition-card:hover {
            transform: translateY(-10px);
        }
        
.tradition-image {
            height: 200px;
            overflow: hidden;
        }
                .tradition-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
.tradition-card:hover .tradition-image img {
            transform: scale(1.1);
        }
                .tradition-content {
            padding: 20px;
        }
        
.tradition-content h3 {
            color: #bc002d;
            margin-bottom: 10px;
        }
                /* Gastronomia */
        .gastronomy {
            background-color: #f9f9f9;
        }
        
.food-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
                .food-item {
            text-align: center;
        }
        
.food-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            overflow: hidden;
            margin: 0 auto 20px;
            border: 5px solid #bc002d;
        }
                .food-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
.food-item h3 {
            margin-bottom: 10px;
            color: #bc002d;
        }
                /* Festivais */
        .festivals {
            background-color: #fff;
        }
        
.festival-timeline {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
        }
                .festival-timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            top: 0;
            bottom: 0;
            width: 4px;
            background-color: #bc002d;
            transform: translateX(-50%);
        }
        
.festival-item {
            margin-bottom: 40px;
            position: relative;
            width: 50%;
            padding: 20px;
        }
                .festival-item:nth-child(odd) {
            left: 0;
        }
        
.festival-item:nth-child(even) {
            left: 50%;
        }
                .festival-content {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        
.festival-content::after {
            content: '';
            position: absolute;
            top: 20px;
            width: 20px;
            height: 20px;
            background-color: white;
            transform: rotate(45deg);
        }
                .festival-item:nth-child(odd) .festival-content::after {
            right: -10px;
        }
        
.festival-item:nth-child(even) .festival-content::after {
            left: -10px;
        }
                .festival-item h3 {
            color: #bc002d;
            margin-bottom: 10px;
        }
        
/* Contato */
        .contact {
            background-color: #f9f9f9;
        }
                .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
.form-group {
            margin-bottom: 20px;
        }
                .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
.form-group input,
        .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
                .form-group textarea {
            height: 150px;
            resize: vertical;
        }
        
.btn {
            display: inline-block;
            background-color: #bc002d;
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: 500;
            transition: background-color 0.3s;
        }
                .btn:hover {
            background-color: #a00024;
        }
        
/* Rodapé */
        footer {
            background-color: #333;
            color: white;
            padding: 40px 0 20px;
        }
                .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        
.footer-section {
            flex: 1;
            min-width: 250px;
            margin-bottom: 20px;
        }
                .footer-section h3 {
            margin-bottom: 20px;
            color: #ffd700;
        }
        
.footer-section ul {
            list-style: none;
        }
                .footer-section ul li {
            margin-bottom: 10px;
        }
        
.footer-section ul li a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }
                .footer-section ul li a:hover {
            color: #ffd700;
        }
        
.social-links {
            display: flex;
            gap: 15px;
        }
                .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
.social-links a:hover {
            color: #ffd700;
        }
                .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #555;
            font-size: 0.9rem;
            color: #aaa;
        }
        
/* Responsividade */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
                        nav ul {
                margin-top: 20px;
                justify-content: center;
            }
            
.banner-content h1 {
                font-size: 2.5rem;
            }
            
 .about-content {
                flex-direction: column;
            }
                        .festival-timeline::before {
                left: 20px;
            }
            
.festival-item {
                width: 100%;
                left: 0 !important;
                padding-left: 50px;
            }
                        .festival-item:nth-child(odd) .festival-content::after,
            .festival-item:nth-child(even) .festival-content::after {
                left: -10px;
                right: auto;
            }
        }
    </style>
</head>
<body>
    <-- Cabeçalho -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <span>日本文化</span>
                </div>
                <nav>
                    <ul>
                        <li><a href="#sobre">Sobre</a></li>
                        <li><a href="#tradicoes">Tradições</a></li>
                        <li><a href="#gastronomia">Gastronomia</a></li>
                        <li><a href="#festivais">Festivais</a></li>
                        <li><a href="#contato">Contato</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

<-- Banner -->
    <section class="banner">
        <div class="container">
            <div class="banner-content">
                <h1>Cultura Japonesa</h1>
                <p>Descubra a riqueza e a beleza da cultura milenar do Japão, onde tradição e modernidade se encontram em perfeita harmonia.</p>
            </div>
        </div>
    </section>

<-- Sobre -->
    <section id="sobre">
        <div class="container">
            <div class="section-title">
                <h2>Sobre a Cultura Japonesa</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <p>A cultura japonesa é uma das mais ricas e fascinantes do mundo, com uma história que remonta a milhares de anos. Ela combina tradições ancestrais com inovações modernas, criando uma sociedade única que valoriza tanto a harmonia quanto o progresso.</p>
                    <p>Do delicado ritual do chá às vibrantes festividades dos matsuri, da precisão das artes marciais à beleza efêmera das flores de cerejeira, a cultura japonesa oferece uma visão profunda de valores como respeito, disciplina e apreciação da beleza na simplicidade.</p>
                    <p>Neste site, exploraremos alguns dos aspectos mais marcantes desta cultura fascinante, desde suas tradições seculares até sua culinária mundialmente famosa.</p>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Templo japonês">
                </div>
            </div>
        </div>
    </section>

 <-- Tradições -->
    <section id="tradicoes" class="traditions">
        <div class="container">
            <div class="section-title">
                <h2>Tradições Japonesas</h2>
            </div>
            <div class="traditions-grid">
                <div class="tradition-card">
                    <div class="tradition-image">
                        <img src="https://images.unsplash.com/photo-1560829589-bf6d65d80d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Cerimônia do chá">
                    </div>
                    <div class="tradition-content">
                        <h3>Cerimônia do Chá</h3>
                        <p>O Chadō, ou "Caminho do Chá", é uma tradição cultural japonesa que envolve a preparação cerimonial e o consumo de matcha. É uma prática que enfatiza harmonia, respeito, pureza e tranquilidade.</p>
                    </div>
                </div>
                <div class="tradition-card">
                    <div class="tradition-image">
                        <img src="https://images.unsplash.com/photo-1587332278432-1838d8cc8a1a?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Arranjo floral">
                    </div>
                    <div class="tradition-content">
                        <h3>Ikebana</h3>
                        <p>A arte japonesa do arranjo floral, conhecida como Ikebana, vai além da simples decoração. É uma disciplina espiritual que busca criar harmonia entre o céu, a terra e a humanidade através da disposição cuidadosa de flores e galhos.</p>
                    </div>
                </div>
                <div class="tradition-card">
                    <div class="tradition-image">
                        <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Caligrafia japonesa">
                    </div>
                    <div class="tradition-content">
                        <h3>Shodō</h3>
                        <p>Shodō, a arte da caligrafia japonesa, é muito mais do que escrever belamente. É uma prática meditativa que exige concentração total e expressa a personalidade e estado de espírito do calígrafo através de pinceladas fluidas e precisas.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

 <-- Gastronomia -->
    <section id="gastronomia" class="gastronomy">
        <div class="container">
            <div class="section-title">
                <h2>Gastronomia Japonesa</h2>
            </div>
            <div class="food-grid">
                <div class="food-item">
                    <div class="food-image">
                        <img src="https://images.unsplash.com/photo-1579584425555-c3ce17fd4351?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Sushi">
                    </div>
                    <h3>Sushi</h3>
                    <p>Prato icônico da culinária japonesa, o sushi combina arroz temperado com vinagre com peixe cru e outros ingredientes. Uma verdadeira arte culinária.</p>
                </div>
                <div class="food-item">
                    <div class="food-image">
                        <img src="https://images.unsplash.com/photo-1563245372-5a5f468a0e6f?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Ramen">
                    </div>
                    <h3>Ramen</h3>
                    <p>Macarrão em caldo saboroso, geralmente acompanhado de carne, ovos cozidos e vegetais. Cada região do Japão tem sua variação única.</p>
                </div>
                <div class="food-item">
                    <div class="food-image">
                        <img src="https://images.unsplash.com/photo-1553621042-f6e147245754?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Tempura">
                    </div>
                    <h3>Tempura</h3>
                    <p>Alimentos empanados e fritos levemente, resultando em uma crosta crocante e fina. Uma técnica culinária introduzida por portugueses no século XVI.</p>
                </div>
                <div class="food-item">
                    <div class="food-image">
                        <img src="https://images.unsplash.com/photo-1585032226657-84dac4d1d6ee?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Wagashi">
                    </div>
                    <h3>Wagashi</h3>
                    <p>Doces tradicionais japoneses frequentemente servidos com chá. São verdadeiras obras de arte que refletem as estações do ano.</p>
                </div>
            </div>
        </div>
    </section>

<-- Festivais -->
    <section id="festivais" class="festivals">
        <div class="container">
            <div class="section-title">
                <h2>Festivais Japoneses</h2>
            </div>
            <div class="festival-timeline">
                <div class="festival-item">
                    <div class="festival-content">
                        <h3>Hanami</h3>
                        <p>O festival de contemplação das flores de cerejeira (sakura) ocorre na primavera, geralmente entre março e maio. Famílias e amigos se reúnem sob as árvores para piqueniques e celebrações.</p>
                    </div>
                </div>
                <div class="festival-item">
                    <div class="festival-content">
                        <h3>Gion Matsuri</h3>
                        <p>Realizado em Kyoto durante todo o mês de julho, é um dos festivais mais famosos do Japão, conhecido por seus desfiles de carros alegóricos ornamentados (yamaboko).</p>
                    </div>
                </div>
                <div class="festival-item">
                    <div class="festival-content">
                        <h3>Tanabata</h3>
                        <p>Festival das estrelas celebrado em 7 de julho, baseado em uma lenda chinesa sobre duas estrelas lovers separadas pela Via Láctea que só podem se encontrar uma vez por ano.</p>
                    </div>
                </div>
                <div class="festival-item">
                    <div class="festival-content">
                        <h3>Obon</h3>
                        <p>Festival budista para honrar os espíritos dos ancestrais, realizado em meados de agosto. Inclui danças tradicionais (bon odori) e a soltura de lanternas nos rios.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

<-- Contato -->
