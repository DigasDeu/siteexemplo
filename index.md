<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lúria - Fabricação de Bonecas</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- TELA DE INTRODUÇÃO -->
<div id="intro">
  <img src="logo.png" alt="Logo Lúria" id="intro-logo">
</div>

<!-- NAVBAR -->
<nav>
  <img src="logo.png" alt="Logo Lúria" class="logo" id="nav-logo">
  <div class="menu">
    <a href="#proposta">Proposta</a>
    <a href="#clientes">Clientes</a>
    <a href="#canais">Canais</a>
    <a href="#contato">Contato</a>
  </div>
</nav>

<!-- HEADER -->
<header>
  <h1>Bem-vindo à Lúria</h1>
  <p>Bonecas que contam histórias e espalham representatividade.</p>
</header>

<!-- MAIN CONTENT -->
<main>

  <section id="proposta">
    <h2>Proposta de Valor</h2>
    <p>Na Lúria, acreditamos que todas as crianças e colecionadores merecem bonecas que celebrem sua identidade, com muita qualidade e carinho.</p>
  </section>

  <section id="clientes">
    <h2>Segmentos de Clientes</h2>
    <p>Atendemos o público infantil, juvenil e colecionadores que buscam bonecas únicas, representativas e encantadoras.</p>
  </section>

  <section id="canais">
    <h2>Canais</h2>
    <p>Estamos presentes nos melhores canais digitais para ouvir você: Instagram, WhatsApp e um atendimento personalizado em nosso site.</p>
  </section>

  <section id="contato">
    <h2>Contato</h2>
    <p>Quer falar conosco, mandar sugestões ou simplesmente conhecer mais sobre a Lúria? Vem bater um papo com a gente!</p>
    <a href="#" class="button">Fale Conosco</a>
    <div class="social-icons">
      <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
      <a href="#" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
    </div>
  </section>

</main>

<!-- FOOTER -->
<footer>
  Obrigada(o) pela atenção! © 2025 Lúria
</footer>

<!-- JS para animação do scroll e da introdução -->
<script>
  // Aparecer sections conforme scroll
  const sections = document.querySelectorAll('section');
  window.addEventListener('scroll', () => {
    const triggerBottom = window.innerHeight * 0.85;
    sections.forEach(section => {
      const boxTop = section.getBoundingClientRect().top;
      if (boxTop < triggerBottom) {
        section.classList.add('animate');
      }
    });
  });

  // Animação da logo
  window.addEventListener('load', () => {
    setTimeout(() => {
      document.getElementById('intro').style.opacity = '0';
      document.getElementById('intro').style.transform = 'scale(1.2)';
    }, 1500);

    setTimeout(() => {
      document.getElementById('intro').style.display = 'none';
    }, 2500);
  });
</script>

</body>
</html>
