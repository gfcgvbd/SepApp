<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App de Salud Infantil</title>
    <style>
        /* Estilos generales para móviles */
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #1a237e, #6a1b9a); /* Fondo degradado */
            color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Para centrar verticalmente */
        }

        .container {
            width: 100%;
            max-width: 380px; /* Ancho máximo para no sobresalir en móviles */
            margin: 0 auto;
            padding: 20px;
            text-align: center;
            background-color: rgba(255, 255, 255, 0.1); /* Fondo transparente en la caja */
            border-radius: 10px;
        }

        h1, h2 {
            margin-top: 20px;
            font-size: 2rem;
        }

        .card {
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            color: #000;
        }

        .form-group {
            margin-bottom: 15px;
            text-align: left;
        }

        input, textarea, button {
            width: 90%; /* Para que los inputs no sobresalgan */
            padding: 12px;
            margin: 10px auto;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            display: block; /* Para centrarlos horizontalmente */
        }

        input, textarea {
            background-color: #f0f0f0;
            color: #000;
        }

        button {
            background-color: #1a237e;
            color: #fff;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #303f9f;
        }

        .welcome {
            font-size: 1.2rem;
            margin-top: 20px;
            margin-bottom: 20px;
        }

        footer {
            margin-top: 30px;
            font-size: 0.9rem;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 15px;
            text-align: center;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            color: #000;
            width: 100%;
            position: relative;
            bottom: 0;
        }

        @media (max-width: 600px) {
            h1, h2 {
                font-size: 1.8rem;
            }

            .card {
                padding: 15px;
                margin: 15px 0;
            }

            button {
                font-size: 1rem;
                padding: 10px;
            }

            input, textarea {
                padding: 10px;
                font-size: 1rem;
            }
        }

        .contact-info {
            margin-top: 20px;
            font-size: 1rem;
            text-align: center;
            color: #000;
            background-color: rgba(255, 255, 255, 0.9);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .contact-info a {
            color: #1a237e;
            text-decoration: none;
        }

        .section {
            margin: 30px 0;
        }

        .section h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .section p {
            font-size: 1rem;
            margin-bottom: 10px;
        }

        .recipes-list {
            text-align: left;
        }

        .recipes-list ul {
            padding-left: 20px;
        }

        .recipes-list li {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>SepApp</h1>
        <h2>App de Salud Infantil</h2>

        <div class="card">
            <h3>Regístrate</h3>
            <div class="form-group">
                <label for="email">Correo electrónico</label>
                <input type="email" id="email" placeholder="Correo electrónico">
            </div>
            <div class="form-group">
                <label for="password">Contraseña</label>
                <input type="password" id="password" placeholder="Contraseña">
            </div>
            <button>Registrarse</button>
        </div>

        <div class="card">
            <h3>Iniciar Sesión</h3>
            <div class="form-group">
                <label for="login-email">Correo electrónico</label>
                <input type="email" id="login-email" placeholder="Correo electrónico">
            </div>
            <div class="form-group">
                <label for="login-password">Contraseña</label>
                <input type="password" id="login-password" placeholder="Contraseña">
            </div>
            <button>Entrar</button>
        </div>

        <p class="welcome">Bienvenido</p>
        <p>La salud de su niño está en nuestras manos. Gracias por usar nuestra app para monitorear su bienestar.</p>

        <div class="card section">
            <h3>Datos del Niño</h3>
            <div class="form-group">
                <label for="nombre">Nombre del niño</label>
                <input type="text" id="nombre" placeholder="Nombre del niño">
            </div>
            <div class="form-group">
                <label for="edad">Edad</label>
                <input type="number" id="edad" placeholder="Edad">
            </div>
        </div>

        <!-- Sección de Recetas -->
        <div class="card section recipes-list">
            <h3>Recetas Saludables</h3>
            <ul>
                <li>Puré de frutas frescas</li>
                <li>Papillas de verduras y pollo</li>
                <li>Sopas nutritivas para niños</li>
            </ul>
        </div>

        <!-- Sección de Alimentación -->
        <div class="card section">
            <h3>Información sobre la Alimentación</h3>
            <p>Es importante ofrecer alimentos variados y equilibrados para que el niño reciba todos los nutrientes necesarios para su crecimiento y desarrollo.</p>
            <p>Recomendamos incluir frutas, verduras, proteínas y carbohidratos en cada comida.</p>
        </div>

        <!-- Sección de Contacto -->
        <div class="contact-info">
            <p><strong>Contacto:</strong></p>
            <p>Teléfono: <a href="tel:+51980823626">+51 980 823 626</a></p>
            <p>Correo: <a href="mailto:appdesaludinfantil@gmail.com">appdesaludinfantil@gmail.com</a></p>
        </div>
    </div>

    <footer>
        &copy; 2024 SepApp - Todos los derechos reservados.
    </footer>
</body>
</html>
