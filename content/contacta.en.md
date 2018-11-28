---
url: "contact"
title: "Contact"
menu:
  main:
    name: "Contact"
    weight: 6
    url: "/contact/"
---
If you need help, have a suggestion or have found errors while using our openBVE contents, leave a message here and we will try to find a solution as soon as possible.

<form name="contact" netlify-honeypot="bot-field" netlify>
  <p hidden><label>Don’t fill this out: <input type="text" name="bot-field"/></p>
  <label>Name</label>
  <input type="text" name="name" required>
  <label>Email</label>
  <input type="email" name="email" required>
  <label>Message</label>
  <textarea name="message" required></textarea>
  <div data-netlify-recaptcha></div>
  <button type="submit">Send</button>
</form>
