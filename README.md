<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Maqsood Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: white;
    }

    nav {
      position: fixed;
      width: 100%;
      background: rgba(0, 0, 0, 0.7);
      padding: 15px 0;
      text-align: center;
      z-index: 1000;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      padding: 10px 20px;
      border-radius: 30px;
      transition: 0.3s ease;
      font-weight: 600;
    }

    nav a:hover {
      background: #1abc9c;
      transform: scale(1.1);
    }

    section {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 80px 20px 50px;
      opacity: 0;
      transform: translateY(50px);
      animation: fadeIn 1s forwards;
    }

    section:nth-of-type(1) { animation-delay: 0.2s; }
    section:nth-of-type(2) { animation-delay: 0.4s; }
    section:nth-of-type(3) { animation-delay: 0.6s; }
    section:nth-of-type(4) { animation-delay: 0.8s; }

    @keyframes fadeIn {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    #home {
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    }

    #about {
      background: linear-gradient(to bottom right, #1abc9c, #16a085);
    }

    #projects {
      background: linear-gradient(to bottom right, #111, #333);
    }

    #contact {
      background: linear-gradient(to bottom right, #222, #444);
    }

    h1 {
      font-size: 48px;
      margin-bottom: 20px;
      animation: floatUp 2s ease-out forwards;
    }

    @keyframes floatUp {
      0% { transform: translateY(40px); opacity: 0; }
      100% { transform: translateY(0); opacity: 1; }
    }

    p {
      font-size: 20px;
      max-width: 600px;
      margin: 0 auto 20px;
      animation: fadeText 1.5s ease-in-out forwards;
    }

    @keyframes fadeText {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .button {
      background-color: #1abc9c;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 30px;
      text-decoration: none;
      font-size: 18px;
      transition: 0.3s;
      display: inline-block;
      margin: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }

    .button:hover {
      background-color: #16a085;
      transform: scale(1.05);
    }

    .social-icons {
      margin-top: 20px;
    }

    .social-icons a {
      text-decoration: none;
      margin: 0 10px;
      font-size: 20px;
      padding: 10px 20px;
      border-radius: 30px;
      display: inline-block;
      background: #E1306C;
      color: white;
      transition: 0.3s ease-in-out;
    }

    .social-icons a:hover {
      background: #c13584;
      transform: scale(1.05);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 10px;
      max-width: 400px;
      margin: auto;
      animation: fadeIn 2s forwards;
    }

    input, textarea {
      padding: 10px;
      border: none;
      border-radius: 5px;
      font-size: 16px;
    }

    footer {
      background: #000;
      color: #aaa;
      text-align: center;
      padding: 20px;
      animation: fadeIn 2s forwards;
    }

    @media (max-width: 768px) {
      h1 { font-size: 32px; }
      p { font-size: 16px; }
      nav a { font-size: 14px; padding: 8px 14px; }
    }
  </style>
</head>
<body>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About Me</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="home">
    <div>
      <h1>Hi, I'm Maqsood</h1>
      <p>Cloud & DevOps Engineer | AWS | Linux | Python</p>
      <a class="button" href="Maqsood_Resume.pdf" download>📄 Download Resume</a>
    </div>
  </section>

  <section id="about">
    <div>
      <h1>About Me</h1>
      <p>I’m passionate about cloud technologies and automation. I work with AWS, DevOps, and Linux systems to deliver real-world solutions.</p>
    </div>
  </section>

  <section id="projects">
    <div>
      <h1>Projects</h1>
      <p>🔐 High-Security ATM System<br>☁️ AWS Cloud Setup for Startup<br>🖥️ Linux Server Automation</p>
    </div>
  </section>

  <section id="contact">
    <div>
      <h1>Contact Me</h1>
      <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message" rows="4" required></textarea>
        <button type="submit" class="button">Send Message</button>
      </form>
      <div class="social-icons">
        <a href="https://wa.me/8111815912?text=Hi%20Maqsood%2C%20I%20saw%20your%20portfolio%20and%20would%20like%20to%20talk!" target="_blank">💬 WhatsApp</a>
        <a href="https://instagram.com/munna__pp" target="_blank">📸 Instagram</a>
      </div>
    </div>
  </section>

  <footer>
    &copy; 2025 Maqsood Rahiman PP. All rights reserved.
  </footer>

</body>
</html>
