---
title: "Contact Me"
layout: single
permalink: /contact
excerpt: "Contact Me"
author_profile: true

---

## Contact Me

Page is under active development, and may not function as expected.

Please fill out the form below to get in touch with me.

<form id="contact-form" action="https://contact-form-350679746849.us-central1.run.app" method="POST">
  <label for="name">Your Name</label>
  <input type="text" name="name" id="name" required>

  <label for="email">Your Email</label>
  <input type="email" name="email" id="email" required>

  <label for="company">Company Name (Optional)</label>
  <input type="text" name="company" id="company">

  <label for="message">Your Message</label>
  <textarea name="message" id="message" required></textarea>

  <!-- reCAPTCHA token will be added here -->
  <input type="hidden" name="g-recaptcha-response" id="recaptcha-response" required>

  <button type="submit">Send Message</button>
</form>

<script src="https://www.google.com/recaptcha/api.js?render=6LcKBcYqAAAAAFyQKPJwgGjuL52zPtmiNf_loSrr"></script>
<script>
  grecaptcha.ready(function() {
    grecaptcha.execute('6LcKBcYqAAAAAFyQKPJwgGjuL52zPtmiNf_loSrr', { action: 'contact_form' }).then(function(token) {
      document.getElementById('recaptcha-response').value = token;
    });
  });
</script>
