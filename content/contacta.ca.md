---
title: "Contacta"
menu:
  main:
    name: "Contacta"
    weight: 6
    url: "/contacta/"
---
Si necessiteu ajuda, teniu suggeriments o trobeu errors mentre feu servir amb els nostres continguts a l’openBVE, podeu escriure un missatge aquí i ho intentarem resoldre el més aviat possible.

<form name="contact" netlify-honeypot="bot-field" netlify>
  <p hidden><label>Don’t fill this out: <input type="text" name="bot-field"/></p>
  <label>Nom</label>
  <input type="text" name="name" required>
  <label>Correu electrònic</label>
  <input type="email" name="email" required>
  <label>Missatge</label>
  <textarea name="message" required></textarea>
  <button type="submit">Envia</button>
</form>
