---
url: "contacto"
title: "Contacto"
menu:
  main:
    name: "Contacto"
    weight: 6
    url: "/contacto/"
---
Si necessitas ayuda, tienes sugerencias o has encontrado algún error usando nuestros contenidos para openBVE, puedes escribir un mensaje aquí e intentaremos resolverlo lo antes posible.

<form name="contact" netlify-honeypot="bot-field" netlify>
  <p hidden><label>Don’t fill this out: <input type="text" name="bot-field"/></p>
  <label>Nombre</label>
  <input type="text" name="name" required>
  <label>Correo electrónico</label>
  <input type="email" name="email" required>
  <label>Mensaje</label>
  <textarea name="message" required></textarea>
  <button type="submit">Enviar</button>
</form>
