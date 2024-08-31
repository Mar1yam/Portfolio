<template>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<div class="container mb-3 fadein-up">
      <div class="big-circle"></div>
      <div class="form">
        <div class="contact-info">
          <h3 class="title">Let's get in touch!</h3>
          <p class="text">
            Feel free to reach out if you have any questions or just want to connect!
          </p>
        
          <div class="flex justify-center">
            <img class="w-32 rounded-full mb-3 fadein-up" src="https://i.imgur.com/IEohd6X.png" alt="Foto">
          </div>
          <div class="social-media">
  <p>Let's Connect!</p>
  <div class="social-icons">
        <!-- LinkedIn -->
        <a href="https://www.linkedin.com/in/mariyam-m-3989a4224/" target="_blank">
      <i class="fab fa-linkedin-in"></i>
    </a>
    <!-- GitHub -->
    <a href="https://github.com/Mar1yam" target="_blank">
      <i class="fab fa-github"></i>
    </a>
    <!-- Email -->
    <a href="mailto:member.mariyam@gmail.com">
      <i class="fas fa-envelope"></i>
    </a>
    <!-- Resume -->
    <a href="https://doc-00-38-prod-02-apps-viewer.googleusercontent.com/viewer2/prod-02/pdf/hhta9ep5svcqecccbrhrm1e1jubdnure/e57opcm7e5lotvno0dp0r72pg2pq2eej/1725061725000/3/100614821988288310807/APznzaZ7jNCkOchPInlJLAUs4_RCom5d_b3rOMB-t8uc7YYlyKrCzxQ8dHXgRe-pXVVQZ3GAN0XOSiCZVHx-yLP8nN6g2TANCZEZaVYA0iErEs0SR8vH6JCM7JaJjbpaHuGvtmoiF5RmywgvkuntF1ZmJf8SKh8ZFXMplY0LBMJBfhmSk8aQidyak9zPfc5TvWAcFjjnGRm9B1IOBtKEVKCj6b5U-UY8KzfiMI-ojMRH89CMGP2aYPcbsMQMhIZ7T_e-72sHldOEployOpVTAJlRUipMBI5ANLxWsdniGr7SAJrZaAumW1k-kAwheLNFpOigARO5wbeDsv4jLW61JJi14Us6YGsdmo4msU4IyW2_K-0mrcZxTu3pr9J9Ho2zetd34M-2d1e_o8AbjAq6KzA3f_KIzUkYHQ==?authuser=0&nonce=0sfqu2okjbv0e&user=100614821988288310807&hash=9ibu61uj0ge5v7kt6cjgbdc0ueht040v" target="_blank">
      <i class="fas fa-file-alt"></i>
    </a>
  </div>
</div>

        </div>
        <div class="contact-form">
          <div class="circle two"></div>
          <form
  action="https://formspree.io/f/xqaznoky"
  method="POST"
  autocomplete="off"
>
  <h3 class="title">Contact.</h3>
  
  <div class="input-container">
    <input type="text" name="name" class="input" required />
    <label for="name">Name</label>
    <span>Name</span>
  </div>

  <div class="input-container">
    <input type="email" name="email" class="input" required />
    <label for="email">Email</label>
    <span>Email</span>
  </div>

  <div class="input-container">
    <input name="subject" type="text" class="input" required />
    <label for="subject">Subject</label>
    <span>Subject</span>
  </div>

  <div class="input-container textarea">
    <textarea name="message" class="input" required></textarea>
    <label for="message">Message</label>
    <span>Message</span>
  </div>
  <input type="submit" value="Send" class="btn" />
</form>

        </div>
      </div>
      </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
  place-items: center;
}

/* Container */
.container {
  display: flex;
  align-items: center;
}

/* Form */
.form {
  width: 100%;
  max-width: 800px;
  background-color: #272727;
  border-radius: 10px;
  box-shadow: 0 0 20px 1px rgba(0, 0, 0, 0.1);
  z-index: 1000;
  overflow: hidden;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

/* Contact Form */
.contact-form {
  background-color: #f4c63c70;
  position: relative;
  width: 100%;
}

/* Form Elements */
form {
  padding: 2.3rem 2.2rem;
  position: relative;
}

.title {
  color: #fff;
  font-weight: 600;
  font-size: 1.5rem;
  margin-bottom: 0.7rem;
}

.input-container {
  position: relative;
  margin: 1rem 0;
}

.input {
  width: 100%;
  outline: none;
  border: 2px solid #fafafa;
  background: none;
  padding: 0.6rem 1.2rem;
  color: #fff;
  font-weight: 500;
  font-size: 0.95rem;
  letter-spacing: 1px;
  border-radius: 25px;
  transition: 0.3s;
}

textarea.input {
  padding: 0.8rem 1.2rem;
  min-height: 150px;
  border-radius: 22px;
  resize: none;
  overflow-y: auto;
}

.input-container label {
  position: absolute;
  top: 50%;
  left: 15px;
  transform: translateY(-50%);
  padding: 0 0.4rem;
  font-weight: 400;
  pointer-events: none;
  z-index: 1000;
  transition: 0.3s;
  color: #fafafa;
}

.input-container.textarea label {
  top: 1rem;
  transform: translateY(0);
}

/* Button */
.btn {
  padding: 0.6rem 1.3rem;
  background-color: #fff;
  border: 2px solid #fafafa;
  font-size: 0.95rem;
  line-height: 1;
  border-radius: 25px;
  color: #000000;
  font-weight: 600;
  cursor: pointer;
  transition: 0.3s;
  margin: 0;
  outline: none;
}

.btn:hover {
  background-color: transparent;
  color: #fff;
}

/* Contact Info */
.contact-info {
  padding: 2.3rem 2.2rem;
  position: relative;
}

.contact-info .title {
  color: #dcbb5a70;
}

.text {
  color: #fff;
  margin: 1.5rem 0 2rem 0;
}

.information {
  display: flex;
  color: #fff;
  margin: 0.7rem 0;
  font-size: 0.95rem;
  align-items: center;
}

.icon {
  font-size: 30px;
  color: #dcbb5a70;
  margin-right: 0.7rem;
}

.social-media {
  padding: 2rem 0 0 0;
}

.social-media p {
  color: #fff;
}

.social-icons {
  display: flex;
  margin-top: 0.5rem;
}

.social-icons a {
  width: 35px;
  height: 35px;
  border-radius: 5px;
  background: linear-gradient(45deg, #dcbc5ad5, #dcbb5a70);
  color: #fff;
  line-height: 35px;
  margin-right: 0.5rem;
  transition: 0.4s;
}

.social-icons a:hover {
  transform: scale(1.09);
}

.contact-info::before {
  content: "";
  position: absolute;
  width: 110px;
  height: 110px;
  border: 22px solid #926e14;
  border-radius: 50%;
  bottom: -77px;
  right: 50px;
  opacity: 0.3;
}

.input-container span {
  position: absolute;
  top: 0;
  left: 25px;
  transform: translateY(-50%);
  font-size: 0.8rem;
  padding: 0 0.4rem;
  color: transparent;
  pointer-events: none;
  z-index: 500;
}

.input-container span::before {
  left: 50%;
}

.input-container span::after {
  right: 50%;
}

.input-container.focus label {
  top: 0;
  transform: translateY(-50%);
  left: 25px;
  font-size: 0.8rem;
}

.input-container.focus span::before,
.input-container.focus span::after {
  width: 50%;
  opacity: 1;
}

/* Responsive Styles */
@media (max-width: 850px) {
  .form {
    grid-template-columns: 1fr;
  }

  .contact-info::before {
    bottom: initial;
    top: -72px;
    right: 65px;
    transform: scale(0.95);
  }

  .contact-form::before {
    top: -12px;
    left: initial;
    right: 70px;
  }

  .text {
    margin: 1rem 0 1.5rem 0;
  }

  .social-media {
    padding: 1.5rem 0 0 0;
  }
}

@media (max-width: 480px) {
  .container {
    padding: 1.5rem;
  }

  .contact-info::before {
    display: none;
  }

  form,
  .contact-info {
    padding: 1.7rem 1.6rem;
  }

  .text,
  .information,
  .social-media p {
    font-size: 0.8rem;
  }

  .title {
    font-size: 1.15rem;
  }

  .social-icons a {
    width: 30px;
    height: 30px;
    line-height: 30px;
  }

  .icon {
    font-size: 25px;
  }

  .input {
    padding: 0.45rem 1.2rem;
  }

  .btn {
    padding: 0.45rem 1.2rem;
  }

} </style>