<script>
import Navbar from './components/navbar.svelte';
  import Counter from './lib/Counter.svelte'
</script>

<Navbar />

<main>
  <section class="hero">
    <div class="hero-content">
      <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="true">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="./src/assets/hero.jpg" class="d-block " alt="...">
          </div>
          <div class="carousel-item">
            <img src="./src/assets/hero2.jpg" class="d-block " alt="...">
          </div>
          <div class="carousel-item">
            <img src="./src/assets/hero3.jpg" class="d-block " alt="...">
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    <div class="herotext">
          <h1 class="slogan">Beauty and Elegance Redefined</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Id assumenda ipsa quibusdam accusamus nostrum similique cumque voluptate fugit nihil unde.</p>

          <button>Click Me</button>
          <Counter />

        </div>
    </div>
        
  </section>

<section class="services">
  <div id="services"></div>
  <h2>Our Services</h2>
  <div class="service-item">
    <img src="./src/assets/haircut.png" alt=""  width="70px">
    <h3>Haircuts</h3>
    <p>Get a fresh new look with our expert haircutting services.</p>
  </div>
  <div class="service-item">
    <img src="./src/assets/medicure.png" alt="" width="70px">
    <h3>Manicure and Pedicure</h3>
    <p>Pamper your hands and feet with our relaxing manicure and pedicure treatments.</p>
  </div>
  <div class="service-item">
    <img src="./src/assets/facial.png" alt="" width="70px">
    <h3>Facial Treatments</h3>
    <p>Rejuvenate your skin with our luxurious facial treatments.</p>
  </div>
</section>

<section class="contact-details">
  <div id="contact"></div>
  <h2>Contact Details</h2>
  <div class="contact-person">
    <h3>Thomas</h3>
    <p>Phone: 08123456789</p>
  </div>
  <div class="contact-person">
    <h3>Sekar</h3>
    <p>Phone: 08164829372</p>
  </div>
</section>


</main>

<style>

  main{
    scroll-behavior: smooth;
  }
  
  .hero {
    display: flex; 
    justify-content: center; 
    align-items: center; 
    height: 70vh; 
    background-position: center; 
    color: black;
    margin-top: 150px;
  }
  
  .hero-content {
    padding: 50px;
    text-align: center; 
    border-radius: 10px; 
  }
  .carousel-item img {
  width: 700px; /* Atur lebar yang diinginkan */
  height: auto; /* Atur tinggi yang diinginkan */
  object-fit: cover; /* Pastikan gambar menutupi seluruh area tanpa distorsi */

}
  .hero-content img {
    max-width: 100%;
    height: auto;
  }
  
  .herotext p {
    text-align: center; 
    width: 80%; 
    max-width: 600px; 
    margin: 0 auto; 
    line-height: 1.6; 
  }
  
  .herotext button {
    display: inline-block; 
    background-color: #e91e63; 
    color: white; 
    border: none; 
    border-radius: 5px; 
    padding: 15px 25px; 
    margin-top: 20px; 
    cursor: pointer;
    transition: background-color 0.3s ease; 
  }
  
  .herotext button:hover {
    background-color: #c2185b; 
  }
  
  .services {
    margin-top: 200px;
    padding: 2rem;
    text-align: center; 
  }
  .services h2 {
    margin-bottom: 2rem;
    font-size: 2.5rem;
    color: #333; 
  }
  .service-item {
    display: inline-block; 
    width: 30%; 
    margin: 1rem;
    padding: 1.5rem;
    border: 1px solid #ddd; 
    border-radius: 8px; 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); 
    transition: all 0.3s ease; 
  }
  .service-item:hover {
    transform: translateY(-5px); 
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15); 
  }
  .service-item img {
    margin-bottom: 1rem;
  }
  .service-item h3 {
    margin-bottom: 0.5rem;
    color: #e91e63; 
  }
  .service-item p {
    color: #555; 
    line-height: 1.6; 
  }
  
  
  .contact-details {
    padding: 30px;
    background-color: wheat; 
    display: flex;           
    flex-wrap: wrap;        
    justify-content: center; 
  }
  .contact-details h2 {
    font-size: 2.5em;
    color: #333;
    margin-bottom: 20px;
    text-align: center;
    width: 100%;            
  }
  .contact-person {
    display: inline-block; 
    margin: 20px;
    padding: 20px;
    border: 1px solid #ddd; 
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    width: 250px; 
    text-align: center; 
    transition: transform 0.2s ease, box-shadow 0.2s ease; 
  }
  
  .contact-person:hover {
    transform: translateY(-5px); 
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); 
  }
  .contact-person h3 {
    color: #e91e63; 
    margin-bottom: 10px;
  }
  .contact-person p {
    color: #555;
  }
  
  
  @media (max-width: 768px) { 
    .hero {
      height: 60vh; /* Sesuaikan tinggi hero section */
      margin-bottom: 200px;
  
    }
    .hero-content {
      padding: 30px; /* Kurangi padding */
    }
    .herotext p {
      width: 90%; /* Lebar paragraf */
      font-size: 1rem; /* Ukuran font */
    }
    .services{
      margin-top: 20px;
    }
    .service-item {
      width: 45%; /* Lebar item layanan */
    }
  }
  /* Media query untuk HP */
  @media (max-width: 480px) { 
    .hero {
      height: 50vh; /* Sesuaikan tinggi hero section */
      margin-bottom: 70px;
  
    }
    .hero-content {
      padding: 20px; /* Kurangi padding */
  
    }
    .herotext p {
      width: 100%; /* Lebar paragraf */
      font-size: 0.9rem; /* Ukuran font */
    }
    .services{
      margin-top: 20px;
    }
    .service-item {
      width: 90%; /* Lebar item layanan */
      margin: 0.5rem; /* Margin item layanan */
    }
    .contact-person {
      width: 90%; /* Lebar kontak person */
    }
  }
  
  </style>