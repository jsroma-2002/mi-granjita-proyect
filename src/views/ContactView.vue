<template>
  <section>
    <div class="section-header">
      <div class="container">
        <h2>Contactanos</h2>
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="contact-info">
          <div class="contact-info-item">
            <div class="contact-info-icon">
              <i class="fas fa-home"></i>
            </div>

            <div class="contact-info-content">
              <h4>Direccion</h4>
              <p>
                Pasaje La Ermita 541,<br />
                Callao, Lima
              </p>
            </div>
          </div>

          <div class="contact-info-item">
            <div class="contact-info-icon">
              <i class="fas fa-phone"></i>
            </div>

            <div class="contact-info-content">
              <h4>Telefono</h4>
              <p>936-110-278</p>
            </div>
          </div>

          <div class="contact-info-item">
            <div class="contact-info-icon">
              <i class="fas fa-envelope"></i>
            </div>

            <div class="contact-info-content">
              <h4>Email</h4>
              <p>migranjita@email.com</p>
            </div>
          </div>
        </div>

        <div class="contact-form">
          <form action="" id="contact-form">
            <h2>Envia un mensaje</h2>
            <div class="input-box">
              <input type="text" required="true" name="" />
              <span>Nombre</span>
            </div>

            <div class="input-box">
              <input type="email" required="true" name="" />
              <span>Email</span>
            </div>

            <div class="input-box">
              <textarea required="true" name=""></textarea>
              <span>Escribe su mensaje...</span>
            </div>

            <div class="input-box">
              <input type="submit" value="Enviar" name="" />
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap");

section {
  margin-top: 100px;
  height: 85vh;
  padding-top: 50px;
  padding-bottom: 50px;
}

.container {
  max-width: 1080px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 20px;
  padding-right: 20px;
}

.section-header {
  margin-bottom: 50px;
  text-align: center;
}

.section-header h2 {
  color: #fc036b;
  font-weight: bold;
  font-size: 3em;
  margin-bottom: 20px;
}

.section-header p {
  color: #7c7c7c;
}

.row {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
}

.contact-info {
  width: 50%;
}

.contact-info-item {
  display: flex;
  margin-bottom: 30px;
}

.contact-info-icon {
  height: 70px;
  width: 70px;
  background-color: #fc036b;
  text-align: center;
  border-radius: 50%;
}

.contact-info-icon i {
  font-size: 30px;
  line-height: 70px;
}

.contact-info-content {
  margin-left: 20px;
}

.contact-info-content h4 {
  color: #fc036b;
  font-size: 1.4em;
  margin-bottom: 5px;
}

.contact-info-content p {
  color: #7c7c7c;
  font-size: 1em;
}

.contact-form {
  background-color: #fff;
  padding: 40px;
  width: 45%;
  padding-bottom: 20px;
  padding-top: 20px;
}

.contact-form h2 {
  font-weight: bold;
  font-size: 2em;
  margin-bottom: 10px;
  color: #333;
}

.contact-form .input-box {
  position: relative;
  width: 100%;
  margin-top: 10px;
}

.contact-form .input-box input,
.contact-form .input-box textarea {
  width: 100%;
  padding: 5px 0;
  font-size: 16px;
  margin: 10px 0;
  border: none;
  border-bottom: 2px solid #333;
  outline: none;
  resize: none;
}

.contact-form .input-box span {
  position: absolute;
  left: 0;
  padding: 5px 0;
  font-size: 16px;
  margin: 10px 0;
  pointer-events: none;
  transition: 0.5s;
  color: #666;
}

.contact-form .input-box input:focus ~ span,
.contact-form .input-box textarea:focus ~ span {
  color: #e91e63;
  font-size: 12px;
  transform: translateY(-20px);
}

.contact-form .input-box input[type="submit"] {
  width: 100%;
  background: #484872;
  color: #fff;
  border: none;
  cursor: pointer;
  padding: 10px;
  font-size: 18px;
  border: 1px solid #484872;
  transition: 0.5s;
}

.contact-form .input-box input[type="submit"]:hover {
  background: #fff;
  color: #484872;
}

@media (max-width: 991px) {
  section {
    padding-top: 50px;
    padding-bottom: 50px;
  }

  .row {
    flex-direction: column;
  }

  .contact-info {
    margin-bottom: 40px;
    width: 100%;
  }

  .contact-form {
    width: 100%;
  }
}
</style>
