<template>
  <section class="about-section">
    <div class="about-content">
      <div class="about-info">
        <h2>About Us</h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
          facilis. Laudantium recusandae ratione ducimus. Labore incidunt rerum
          veniam mollitia quasi nemo nesciunt aut id, suscipit enim. Ex saepe
          reiciendis ducimus?
        </p>
      </div>
      <div>
        <div class="about-img">
          <img
            src="https://cachimbo.pe/wp-content/uploads/2021/04/upc.jpg"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  height: 90vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
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
  color: #484872;
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
  color: #7c7c7c;
}
.about-img {
  align-self: center;
  padding: 10px;
  transition: 0.3s;
  width: 250;
  height: 250;
}
</style>
