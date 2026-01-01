<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="D&E Studio">
    <title>D&E Studio | Indie Game Dev</title>
    <style>
        :root {
            --primary-color: #222;
            --secondary-color: #333;
            --accent-color: #007bff; /* Um tom azul sutil para links e destaques */
            --text-color: #333;
            --light-bg: #f8f9fa;
            --light-section: #ffffff;
            --white: #fff;
            --shadow: 0 4px 15px rgba(0,0,0,0.05);
            --border-radius: 12px;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            background-color: var(--light-bg);
            color: var(--text-color);
        }

        /* Cabeçalho Melhorado */
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            padding: 4rem 1rem;
            text-align: center;
        }

        header h1 {
            font-size: 3rem;
            letter-spacing: 2px;
            margin-bottom: 0.5rem;
            text-transform: uppercase;
        }

        /* Navegação */
        nav {
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(5px);
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }

        nav a {
            color: var(--secondary-color);
            text-decoration: none;
            font-weight: 600;
            padding: 0.5rem 1.2rem;
            border-radius: 20px;
            transition: var(--transition);
            font-size: 0.9rem;
        }

        nav a:hover {
            background-color: var(--secondary-color);
            color: var(--white);
        }

        main {
            max-width: 1000px;
            margin: 0 auto;
            padding: 1rem;
        }

        section {
            padding: 4rem 1.5rem;
            margin: 2rem 0;
            background: var(--light-section);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
        }

        h2 {
            font-size: 2.2rem;
            margin-bottom: 2rem;
            color: var(--primary-color);
            text-align: center;
            position: relative;
        }

        h2::after {
            content: '';
            display: block;
            width: 50px;
            height: 4px;
            background: var(--accent-color);
            margin: 10px auto;
            border-radius: 2px;
        }

        /* Team Members */
        .team-members {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .member {
            background: var(--light-bg);
            padding: 2rem;
            border-radius: var(--border-radius);
            text-align: center;
            transition: var(--transition);
            border: 1px solid rgba(0,0,0,0.05);
        }

        .member:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .member h3 {
            font-size: 0.9rem;
            color: #777;
            text-transform: uppercase;
            margin-bottom: 0.5rem;
        }

        .member strong {
            font-size: 1.4rem;
            color: var(--primary-color);
        }

        /* Novidades */
        .novidade {
            border-left: 4px solid var(--primary-color);
            padding: 1.5rem 2rem;
            margin-bottom: 2rem;
            background: #fff;
        }

        .date {
            display: inline-block;
            background: #eee;
            padding: 2px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
            margin-bottom: 1rem;
        }

        .game-features {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            list-style: none;
            margin-top: 1rem;
        }

        .game-features li {
            background: #e9ecef;
            padding: 5px 12px;
            border-radius: 5px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        /* Contato */
        .contact-card {
            background: var(--primary-color);
            color: white;
            padding: 3rem;
            border-radius: var(--border-radius);
            text-align: center;
        }

        .email-link {
            display: inline-block;
            margin-top: 1.5rem;
            color: #fff;
            font-size: 1.2rem;
            text-decoration: none;
            border: 2px solid rgba(255,255,255,0.2);
            padding: 10px 25px;
            border-radius: 30px;
            transition: var(--transition);
        }

        .email-link:hover {
            background: white;
            color: var(--primary-color);
        }

        footer {
            text-align: center;
            padding: 3rem;
            color: #777;
            font-size: 0.9rem;
        }

        @media (max-width: 600px) {
            header h1 { font-size: 2rem; }
            .nav-container { gap: 0.5rem; flex-wrap: wrap; }
            nav a { font-size: 0.8rem; padding: 0.5rem; }
        }
    </style>
</head>
<body>
    <header>
        <h1>D&E Studio</h1>
        <p>Criando experiências independentes</p>
    </header>

    <nav>
        <div class="nav-container">
            <a href="#home">Início</a>
            <a href="#novidades">Novidades</a>
            <a href="#contato">Contato</a>
        </div>
    </nav>

    <main>
        <section id="home">
            <h2>Sobre o Estúdio</h2>
            <p style="text-align: center; margin-bottom: 2rem; color: #666;">
                "Dois caras + Força de Vontade = Um Estúdio independente!"
            </p>
            
            <div class="team-members">
                <div class="member">
                    <h3>Desenvolvedor</h3>
                    <strong>Davi</strong>
                </div>
                <div class="member">
                    <h3>Designer</h3>
                    <strong>Enzo</strong>
                </div>
            </div>
        </section>
        
        <section id="novidades">
            <h2>Novidades</h2>
            
            <article class="novidade">
                <span class="date">30 de Dezembro de 2025</span>
                <h3>Just Move! <small style="color: var(--accent-color);">(Em Testes)</small></h3>
                <p>Um jogo de ação focado em reflexos, onde sobreviver é o seu único objetivo.</p>
                
                <ul class="game-features">
                    <li>- Controles WASD</li>
                    <li>- Power-ups dinâmicos</li>
                    <li>- Inimigos variados</li>
                    <li>- Progressão de Nível</li>
                </ul>
            </article>
            
            <article class="novidade">
                <span class="date">25 de Dezembro de 2025</span>
                <h3>O Início</h3>
                <p>Começo da D&E Studio.</p>
            </article>
        </section>
        
        <section id="contato">
            <div class="contact-card">
                <h2>Contato</h2>
                <p>Tem uma ideia ou feedback? Fale conosco!</p>
                <a href="mailto:davi.phantom07@gmail.com" class="email-link">
                    ✉ davi.phantom07@gmail.com
                </a>
                <p style="margin-top: 1.5rem; opacity: 0.7;">D&E Studio lhe espera!</p>
            </div>
        </section>
    </main>
    
    <footer>
        <p>© 2025 D&E Studio</p>
        <p>Por : Davi e Enzo</p>
    </footer>
</body>
</html>
