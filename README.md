index.html

<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>BrandName</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="logo">BrandName</div>
    <div class="menu-toggle" id="menu-toggle">&#9776;</div>
    <nav id="nav">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#collection">Collezione</a></li>
        <li><a href="#about">Chi siamo</a></li>
        <li><a href="#contact">Contatti</a></li>
      </ul>
    </nav>
  </header>  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Benvenuto su BrandName</h1>
      <p>Nuova collezione in arrivo</p>
    </div>
  </section>  <section id="collection" class="section">
    <h2>Collezione</h2>
    <p>Qui andranno i tuoi prodotti o immagini di moda.</p>
  </section>  <section id="about" class="section">
    <h2>Chi siamo</h2>
    <p>Descrivi qui la missione del tuo brand.</p>
  </section>  <section id="contact" class="section">
    <h2>Contatti</h2>
    <p>Email, social o form di contatto.</p>
  </section>  <footer>
    <p>&copy; 2025 BrandName - Tutti i diritti riservati</p>
  </footer>  <script>
    const toggle = document.getElementById('menu-toggle');
    const nav = document.getElementById('nav');
    toggle.addEventListener('click', () => {
      nav.classList.toggle('open');
    });
  </script></body>
</html>style.css

body { margin: 0; font-family: Arial, sans-serif; background-color: #ffffff; color: #111; }

header { display: flex; justify-content: space-between; align-items: center; padding: 1rem; position: fixed; width: 100%; top: 0; background-color: #fff; border-bottom: 1px solid #ddd; z-index: 10; }

.logo { font-weight: bold; font-size: 1.2rem; }

.menu-toggle { display: none; font-size: 1.5rem; cursor: pointer; }

nav ul { list-style: none; display: flex; gap: 1.5rem; margin: 0; padding: 0; }

nav a { text-decoration: none; color: #111; transition: color 0.3s; }

nav a:hover { color: #555; }

.hero { height: 100vh; background: url('https://via.placeholder.com/1500x800') center/cover no-repeat; display: flex; align-items: center; justify-content: center; text-align: center; }

.hero-content { background-color: rgba(255, 255, 255, 0.8); padding: 2rem; border-radius: 8px; }

.section { padding: 5rem 2rem; max-width: 900px; margin: 0 auto; text-align: center; }

footer { text-align: center; padding: 2rem; border-top: 1px solid #ddd; font-size: 0.9rem; background-color: #f9f9f9; }

@media (max-width: 768px) { .menu-toggle { display: block; } nav ul { display: none; flex-direction: column; background: #fff; position: absolute; top: 60px; left: 0; width: 100%; border-top: 1px solid #ddd; } nav.open ul { display: flex; } }
