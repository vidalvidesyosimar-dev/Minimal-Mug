<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Minimal Mug</title>
  <style>
    :root {
      --primary: #ffffff;
      --accent: #333333;
      --highlight: #d4cfcf;
      --font-main: 'Helvetica', sans-serif;
      --font-secondary: 'Arial', sans-serif;
    }

    body {
      margin: 0;
      padding: 0;
      font-family: var(--font-main);
      background-color: var(--primary);
      color: var(--accent);
    }

    header {
      text-align: center;
      padding: 2rem 1rem;
      background-color: var(--highlight);
      font-size: 2rem;
      font-weight: bold;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      padding: 1rem;
      font-size: 1.1rem;
    }

    nav a {
      text-decoration: none;
      color: var(--accent);
      font-family: var(--font-secondary);
    }

    section {
      max-width: 900px;
      margin: auto;
      padding: 2rem 1rem;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .product {
      border: 1px solid #ccc;
      border-radius: 10px;
      padding: 1rem;
      text-align: center;
      background-color: #f9f9f9;
    }

    .product img {
      width: 100%;
      border-radius: 8px;
    }

    button, .btn-whatsapp {
      margin-top: 10px;
      padding: 0.7rem 1.2rem;
      border: none;
      background-color: var(--accent);
      color: white;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
    }

    .btn-whatsapp {
      display: inline-block;
      text-decoration: none;
      background-color: #25d366;
    }

    form input, form textarea {
      width: 100%;
      padding: 0.8rem;
      margin-bottom: 1rem;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 1rem;
    }
  </style>
</head>
<body>

  <header>Minimal Mug</header>

  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#productos">Productos</a>
    <a href="#contacto">Contacto</a>
    <a href="#pedido">Pedido</a>
  </nav>

  <!-- Inicio -->
  <section id="inicio">
    <h2>Bienvenido a Minimal Mug</h2>
    <p>La tienda de tasas minimalistas pensada para amantes del diseño simple y elegante.</p>
  </section>

  <!-- Productos -->
  <section id="productos">
    <h2>Catálogo de productos</h2>
    <div class="product-grid">

      <div class="product">
        <img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab" alt="Taza blanca minimalista" />
        <h3>Taza Blanca</h3>
        <p>Diseño limpio y elegante.</p>
        <p><strong>$25.000 COP</strong></p>
        <button>Comprar ahora</button>
        <a class="btn-whatsapp" href="https://wa.me/573000000000">Ordenar por WhatsApp</a>
      </div>

      <div class="product">
        <img src="https://images.unsplash.com/photo-1542219550-37153d387c5d" alt="Taza negra minimalista" />
        <h3>Taza Negra</h3>
        <p>Perfecta para un estilo sofisticado.</p>
        <p><strong>$27.000 COP</strong></p>
        <button>Comprar ahora</button>
        <a class="btn-whatsapp" href="https://wa.me/573000000000">Ordenar por WhatsApp</a>
      </div>

      <div class="product">
        <img src="https://images.unsplash.com/photo-1514432324607-a09d9b4aefdd" alt="Taza beige minimalista" />
        <h3>Taza Beige</h3>
        <p>Suavidad y neutralidad en tu mesa.</p>
        <p><strong>$26.000 COP</strong></p>
        <button>Comprar ahora</button>
        <a class="btn-whatsapp" href="https://wa.me/573000000000">Ordenar por WhatsApp</a>
      </div>

    </div>
  </section>

  <!-- Contacto -->
  <section id="contacto">
    <h2>Contacto</h2>
    <p>Escríbenos para dudas o pedidos especiales.</p>
    <form>
      <input type="text" placeholder="Tu nombre" required />
      <input type="email" placeholder="Correo electrónico" required />
      <textarea rows="4" placeholder="Mensaje"></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <!-- Pedido -->
  <section id="pedido">
    <h2>Realizar un pedido</h2>
    <p>Puedes llenar el formulario o pedir directamente por WhatsApp.</p>

    <form>
      <input type="text" placeholder="Nombre" required />
      <input type="text" placeholder="Producto solicitado" required />
      <input type="number" placeholder="Cantidad" required />
      <button type="submit">Enviar pedido</button>
    </form>

    <p>O</p>
    <a class="btn-whatsapp" href="https://wa.me/573000000000">Ordenar por WhatsApp</a>
  </section>

</body>
</html>
