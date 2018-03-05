---
title: "Contacta"
menu:
  main:
    name: "Contacta"
    weight: 6
    url: "/contacta/"
---
Pàgina no disponible temporalment. Disculpeu les molèsties.

<form name="contact" action="/missatge-enviat/" netlify>
  <p hidden>
    <label>Don’t fill this out: <input type="text" name="bot-field"/>
  <p>
  <p>
    <label>Nom: <input type="text" name="name"></label>   
  </p>
  <p>
    <label>Correu electrònic: <input type="email" name="email"></label>
  </p>
  <p>
    <label>Missatge: <textarea name="message"></textarea></label>
  </p>
  <p>
    <button type="submit">Envia</button>
  </p>
</form>
