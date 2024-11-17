<template>
  <section class="waitlist" id="waitlist">
    <h2>Únete a Probar Taxia</h2>
    <p>Completa el Google Form o envíanos un correo a info@taxia.com</p>
    <a href="https://forms.gle/tu_link_al_google_form" target="_blank" class="button">Abre la Forma</a>
  </section>
</template>

<style scoped>
.waitlist {
  padding: 40px 0;
  text-align: center;
}

.waitlist h2 {
  color: #efefef;
  font-size: 1.6em;
}

.waitlist p {
  color: #e0e0e0;
  margin-bottom: 20px;
}

.button {
  display: inline-block;
  padding: 10px 20px;
  background-color: #0733f9;
  color: #ffffff;
  text-decoration: none;
  border-radius: 5px;
  margin: 5px;
  text-align: center;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.button:hover {
  background-color: #e0e0e0;
  color: #000000;
}

/* Responsive Styles */
@media (max-width: 600px) {
  .button {
    width: 100%;
    max-width: 300px;
  }
}
</style>
