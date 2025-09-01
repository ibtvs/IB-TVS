
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>IB TVS</title>

<!-- Fonts -->
<link href="https://fonts.googleapis.com/css2?family=League+Spartan:wght@700&display=swap" rel="stylesheet">

<style>
* { margin:0; padding:0; box-sizing:border-box; font-family:'Roboto', sans-serif; }

/* Body background */
body {
  scroll-behavior: smooth;
  background: linear-gradient(270deg, #b3cde0, #6497b1, #005b96);
  background-size: 600% 600%;
  animation: gradientAnim 20s ease infinite;
  color:white;
  padding-bottom:100px;
}
@keyframes gradientAnim {
  0%{background-position:0% 50%;}
  50%{background-position:100% 50%;}
  100%{background-position:0% 50%;}
}

/* Header */
header {
    text-align:center;
    padding:30px 20px;
    color:white;
    font-size:2.5em;
    font-family: 'League Spartan', sans-serif;
    font-weight: bold;
    background: linear-gradient(90deg, #0d47a1, #c8102e);
    border-radius: 10px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.3);
    position: relative;
}
header::after {
    content: "";
    display: block;
    width: 120px;
    height: 6px;
    margin: 10px auto 0 auto;
    background: linear-gradient(90deg, #00c6ff, #0072ff);
    border-radius: 3px;
}

/* Bikes Section */
section { padding:60px 20px; max-width:1000px; margin:auto; }
.bikes { display:flex; flex-wrap:wrap; justify-content:center; gap:30px; perspective:1000px; }
.bike-card { width:220px; height:180px; position:relative; cursor:pointer; }
.bike-inner { position:relative; width:100%; height:100%; text-align:center; transition: transform 0.8s; transform-style: preserve-3d; }
.bike-front, .bike-back {
  position:absolute; width:100%; height:100%; border-radius:10px;
  backface-visibility: hidden;
  box-shadow:0 6px 15px rgba(0,0,0,0.3);
  display:flex; flex-direction:column; align-items:center; justify-content:center;
  padding:10px;
}
.bike-front { background:#1e2a38; }
.bike-front h3 { color:#ffd700; margin-bottom:5px; }
.bike-front p { font-size:0.9em; color:#ddd; }
.bike-back { background:#283747; color:#ffd700; transform: rotateY(180deg); font-size:0.85em; line-height:1.4em; }

/* Contact Form */
.contact-form { max-width:500px; margin:60px auto; background:#1e2a38; padding:30px; border-radius:10px; box-shadow:0 6px 12px rgba(0,0,0,0.3); }
.contact-form input, .contact-form textarea, .contact-form select {
  width:100%; padding:10px; margin:10px 0; border-radius:5px; border:1px solid #ccc; background:#283747; color:white;
}
.contact-form input::placeholder, .contact-form textarea::placeholder { color:#ccc; }
.contact-form button { background:#ffd700; color:#1e2a38; padding:12px 20px; border:none; border-radius:5px; cursor:pointer; font-weight:bold;}
.contact-form button:disabled { background:gray; cursor:not-allowed; }
.contact-form button:hover:not(:disabled) { background:#e6c200; }
#form-msg { text-align:center; margin-top:10px; color:#ffd700; }

/* Footer fixed */
footer { background: linear-gradient(90deg, #0d47a1, #c8102e); color:white; text-align:center; padding:10px; position:fixed; bottom:0; left:0; right:0; }
footer p { margin:3px 0; }

/* WhatsApp Button */
#whatsapp-btn { position: fixed; bottom:80px; right:20px; background:#25D366; color:white; border-radius:50%; width:60px; height:60px; display:flex; justify-content:center; align-items:center; font-size:30px; box-shadow:0 4px 6px rgba(0,0,0,0.3); cursor:pointer; z-index:1000; transition: transform 0.3s;}
#whatsapp-btn:hover { transform: scale(1.1); }

/* Responsive */
@media(max-width:768px){ .bikes { flex-direction:column; align-items:center; } }
</style>
</head>
<body>

<header>IB TVS</header>

<section id="bikes">
<div class="bikes">

<!-- Bike Cards -->
<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS XL100</h3><p>"Ride simple, ride smart."</p></div>
    <div class="bike-back">"Efficiency is the real style."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Apache RTR 160</h3><p>"Power meets style."</p></div>
    <div class="bike-back">"Feel the thrill of every curve."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Jupiter</h3><p>"Comfort on every ride."</p></div>
    <div class="bike-back">"Smooth journeys create happy memories."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Raider 125</h3><p>"Modern ride, modern you."</p></div>
    <div class="bike-back">"Innovation in every detail."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Ntorq</h3><p>"Speed with attitude."</p></div>
    <div class="bike-back">"Every ride is a statement."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS iQube</h3><p>"Silent, smart, electric."</p></div>
    <div class="bike-back">"Future is electric, ride the change."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Radeon</h3><p>"Classic comfort."</p></div>
    <div class="bike-back">"Tradition meets reliability."</div>
  </div>
</div>

<div class="bike-card">
  <div class="bike-inner">
    <div class="bike-front"><h3>TVS Sport</h3><p>"Economical and reliable."</p></div>
    <div class="bike-back">"Smart choices, happy rides."</div>
  </div>
</div>

</div>
</section>

<section id="contact">
<h2>Contact Us</h2>
<form class="contact-form">
<input type="text" name="name" placeholder="Your Name" required>
<input type="email" name="email" placeholder="Your Email" required>
<input type="tel" name="number" placeholder="Your Phone Number" required>
<select name="bike" required>
  <option value="">Select Bike</option>
  <option value="XL100">TVS XL100</option>
  <option value="Apache RTR 160">TVS Apache RTR 160</option>
  <option value="Jupiter">TVS Jupiter</option>
  <option value="Raider 125">TVS Raider 125</option>
  <option value="Ntorq">TVS Ntorq</option>
  <option value="iQube">TVS iQube</option>
  <option value="Radeon">TVS Radeon</option>
  <option value="Sport">TVS Sport</option>
</select>
<textarea name="message" placeholder="Your Comment" rows="5" required></textarea>
<button type="submit">Send Message</button>
<p id="form-msg"></p>
</form>
</section>

<footer>
<p>© 2025 IB TVS | Email: ibtvs2025@gmail.com</p>
<p>📞 <a href="tel:+917348589452" style="color:white; text-decoration:none;">+91 73485 89452</a></p>
</footer>

<div id="whatsapp-btn" onclick="window.open('https://wa.me/917348589452','_blank')">💬</div>

<script src="https://cdn.emailjs.com/dist/email.min.js"></script>
<script>
(function(){ emailjs.init("-2KUdC3STqIMMkIZq"); })();
const form = document.querySelector('.contact-form');
const submitBtn = form.querySelector('button');
const formMsg = document.getElementById('form-msg');

form.addEventListener('submit', function(e){
    e.preventDefault();
    submitBtn.disabled = true;
    formMsg.textContent = '';
    emailjs.sendForm('service_q3knu7o','template_2qb9f0s',this)
    .then(function(){
        formMsg.style.color = 'lightgreen';
        formMsg.innerHTML = '✅ Message sent successfully!';
        form.reset();
    })
    .catch(function(error){
        formMsg.style.color = 'red';
        formMsg.innerHTML = '❌ Failed to send message: ' + error.text;
    })
    .finally(function(){ submitBtn.disabled = false; });
});

// Flip cards
const cards = document.querySelectorAll('.bike-card');
cards.forEach(card => {
    card.addEventListener('click', () => {
        const inner = card.querySelector('.bike-inner');
        if(inner.style.transform === 'rotateY(180deg)'){
            inner.style.transform = 'rotateY(0deg)';
        } else {
            inner.style.transform = 'rotateY(180deg)';
        }
    });
});
</script>
</body>
</html>
