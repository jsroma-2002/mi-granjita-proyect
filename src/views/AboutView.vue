<template>
  <section class="about-section">
    <div class="about-content">
      <div class="about-info">
        <h2>Nosotros</h2>
        <p>
          Mi granjita es un proyecto elabora por estudiantes la UPC(universidad peruana de ciencias aplicadas).
          Tenemos el proposito de ofrecer una experiencia vivencial en la naturaleza para todas las personas y familias que sientan
          que la dinamica urbana empeora su salud y rutina diaria. Nuestra propuesta es integrar a estas familias en la vida campestre
          de una manera segura, confiable y comoda.
        </p>
      </div>
      <div>
        <div class="about-img">
          <img
            src="https://cdn.discordapp.com/attachments/833172117566259241/984344542532763668/unknown.png"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  margin-top: 8vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  background-color: #ffffff;
}
.about-content {
  margin: 60px 100px;
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}
.about-info {
  max-width: 650px;
  padding-bottom: 25px;
}
.about-info h2 {
  color: #666785;
  font-size: 55px;
  text-transform: uppercase;
  font-weight: 800;
  letter-spacing: 2px;
  line-height: 60px;
  margin-bottom: 30px;
}
.about-info p {
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 40px;
}
.about-img {
  align-self: center;
  padding: 10px;
  transition: 0.3s;
  width: 250;
  height: 250;
}
</style>