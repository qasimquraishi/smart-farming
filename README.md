<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>AgriSmart | Agriculture Made Smart</title>
<style>
  /* Basic reset and style */
  * { box-sizing: border-box; }
  body {
    font-family: Arial, sans-serif;
    margin: 0; padding: 0;
    background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1470&q=80') no-repeat center center fixed;
    background-size: cover;
    color: #1b3a1a;
  }
  header {
    background: rgba(46,125,50,0.9);
    padding: 10px 20px;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  nav a {
    color: white;
    margin: 0 10px;
    text-decoration: none;
    font-weight: bold;
    cursor: pointer;
  }
  nav a.active, nav a:hover {
    background: #a3d38a;
    color: #1b3a1a;
    padding: 5px 10px;
    border-radius: 5px;
  }
  .welcome-text {
    font-weight: bold;
  }
  main {
    background: rgba(255,255,255,0.95);
    max-width: 1000px;
    margin: 30px auto;
    padding: 20px;
    border-radius: 12px;
    min-height: 70vh;
  }
  section {
    display: none;
  }
  section.active {
    display: block;
  }
  h2 {
    color: #2e7d32;
    text-align: center;
  }
  .grid {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
  }
  .card {
    background: #f7fff7;
    border-radius: 10px;
    padding: 15px;
    width: 220px;
    box-shadow: 0 0 10px #a3d38a99;
    text-align: center;
  }
  .card img {
    width: 100%;
    height: 140px;
    object-fit: cover;
    border-radius: 10px;
    margin-bottom: 10px;
  }
  /* Form styling */
  form {
    max-width: 400px;
    margin: 0 auto;
  }
  label {
    font-weight: bold;
    display: block;
    margin: 10px 0 5px;
  }
  input {
    width: 100%;
    padding: 8px;
    border-radius: 6px;
    border: 1.5px solid #a3d38a;
  }
  button {
    margin-top: 15px;
    padding: 12px;
    width: 100%;
    background: #4caf50;
    color: white;
    border: none;
    font-weight: bold;
    border-radius: 8px;
    cursor: pointer;
  }
  button:hover {
    background: #81c784;
  }
  .message {
    margin-top: 10px;
    text-align: center;
    font-weight: bold;
  }
</style>
</head>
<body>

<header>
  <nav>
    <a href="#" class="active" data-section="home">Home | گھر</a>
    <a href="#" data-section="tools">Agri Tools | زرعی آلات</a>
    <a href="#" data-section="ai">AI Features | مصنوعی ذہانت</a>
    <a href="#" data-section="sell">Sell Crops | فصل فروخت کریں</a>
    <a href="#" data-section="about">About | ہمارے بارے میں</a>
  </nav>
  <div class="welcome-text">Welcome to AgriSmart | ایگری سمارٹ میں خوش آمدید</div>
</header>

<main>
  <!-- Home / Seeds + Sign In -->
  <section id="home" class="active" tabindex="0">
    <h2>Popular Seeds & Prices | مقبول بیج اور قیمتیں</h2>
    <div class="grid">
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2016/03/27/20/55/wheat-1283500_1280.jpg" alt="Wheat" />
        <h3>Wheat | گندم</h3>
        <p>Price: ₨ 4500 / quintal</p>
      </div>
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2017/07/31/16/36/rice-2555152_1280.jpg" alt="Rice" />
        <h3>Rice | چاول</h3>
        <p>Price: ₨ 5200 / quintal</p>
      </div>
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2017/05/03/17/33/corn-2280549_1280.jpg" alt="Corn" />
        <h3>Corn | مکئی</h3>
        <p>Price: ₨ 4700 / quintal</p>
      </div>
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2015/03/26/09/47/potatoes-690132_1280.jpg" alt="Potato" />
        <h3>Potato | آلو</h3>
        <p>Price: ₨ 4000 / quintal</p>
      </div>
    </div>
    <hr />
    <div style="max-width: 400px; margin: 30px auto; background:#eaf5df; padding:20px; border-radius:12px;">
      <h3>Sign In | لاگ ان کریں</h3>
      <form id="signin-form" novalidate>
        <label for="username">Username | صارف نام</label>
        <input type="text" id="username" name="username" placeholder="Username" required />
        <label for="password">Password | پاس ورڈ</label>
        <input type="password" id="password" name="password" placeholder="Password" required />
        <button type="submit">Sign In | لاگ ان کریں</button>
        <p id="signin-msg" class="message" role="alert"></p>
      </form>
    </div>
  </section>

  <!-- Agri Tools -->
  <section id="tools" tabindex="0">
    <h2>Agri Tools & Prices | زرعی آلات اور قیمتیں</h2>
    <div class="grid">
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2017/01/20/00/30/tractor-1992524_1280.jpg" alt="Tractor" />
        <h3>Tractor | ٹریکٹر</h3>
        <p>Price: ₨ 2,500,000</p>
      </div>
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2017/08/07/06/17/plough-2596996_1280.jpg" alt="Plough" />
        <h3>Plough | ہل</h3>
        <p>Price: ₨ 30,000</p>
      </div>
      <div class="card">
        <img src="https://cdn.pixabay.com/photo/2016/07/12/11/04/harvester-1502469_1280.jpg" alt="Harvester" />
        <h3>Harvester | ہارویسٹر</h3>
        <p>Price: ₨ 1,200,000</p>
      </div>
    </div>
  </section>

  <!-- AI Features -->
  <section id="ai" tabindex="0">
    <h2>AI Features | مصنوعی ذہانت</h2>
    <ul style="max-width: 600px; margin: auto; padding-left: 20px;">
      <li>☀️ <strong>Weather Prediction:</strong> Accurate localized forecasts for irrigation and harvest planning.</li>
      <li>🛡️ <strong>Pest & Disease Detection:</strong> Early identification using image recognition.</li>
      <li>💧 <strong>Resource Optimization:</strong> AI-driven fertilizer and water recommendations.</li>
      <li>📈 <strong>Market Forecasting:</strong> Price predictions to maximize profits.</li>
    </ul>
  </section>

  <!-- Sell Crops -->
  <section id="sell" tabindex="0">
    <h2>Sell Your Crops | اپنی فصل فروخت کریں</h2>
    <form id="sell-form" novalidate style="max-width:400px; margin:auto;">
      <label for="crop-name">Crop Name | فصل کا نام</label>
      <input type="text" id="crop-name" name="crop-name" required placeholder="مثلاً: گندم" />
      <label for="quantity">Quantity (quintals) | مقدار (کوئنٹل)</label>
      <input type="number" id="quantity" name="quantity" required min="1" placeholder="مثلاً: 10" />
      <label for="contact">Contact Number | رابطہ نمبر</label>
      <input type="tel" id="contact" name="contact" required pattern="[0-9]{10,13}" placeholder="03001234567" />
      <button type="submit">Submit | جمع کریں</button>
      <p id="sell-msg" class="message" role="alert"></p>
    </form>
  </section>

  <!-- About -->
  <section id="about" tabindex="0">
    <h2>About AgriSmart | ایگری سمارٹ کے بارے میں</h2>
    <p style="max-width:700px; margin:auto; line-height:1.5;">
      AgriSmart ایک جدید ایپ ہے جو کسانوں کی مدد کے لیے بنائی گئی ہے۔ یہ بیجوں کی قیمتیں، زرعی آلات، اور مصنوعی ذہانت کی مدد سے بہترین زراعتی فیصلے کرنے میں مدد دیتی ہے۔  
      ہم کسانوں پر اعتماد اور ایمان رکھتے ہیں کہ جدید ٹیکنالوجی کے ذریعے ہم ملک کی زرعی ترقی میں اہم کردار ادا کر سکتے ہیں۔  
      ہمارا مقصد کسانوں کو جدید معلومات فراہم کرنا اور ان کی محنت کو زیادہ منافع بخش بنانا ہے۔
    </p>
  </section>
</main>

<script>
  // نیویگیشن کام کرے، بٹن کلک پر متعلقہ سیکشن دکھائے
  document.addEventListener('DOMContentLoaded', () => {
    const navLinks = document.querySelectorAll('nav a');
    const sections = document.querySelectorAll('main section');

    navLinks.forEach(link => {
      link.addEventListener('click', e => {
        e.preventDefault();
        // active کلاس نکالیں
        navLinks.forEach(l => l.classList.remove('active'));
        link.classList.add('active');

        const target = link.getAttribute('data-section');
        sections.forEach(sec => sec.classList.remove('active'));

        const targetSection = document.getElementById(target);
        if(targetSection){
          targetSection.classList.add('active');
          targetSection.focus();
        }
      });
    });

    // Sign In فارم
    const signinForm = document.getElementById('signin-form');
    const signinMsg = document.getElementById('signin-msg');

    signinForm.addEventListener('submit', e => {
      e.preventDefault();
      const username = signinForm.username.value.trim();
      const password = signinForm.password.value.trim();

      if (!username || !password) {
        signinMsg.style.color = 'red';
        signinMsg.textContent = 'Please enter both username and password | براہ کرم دونوں خانے پر کریں۔';
        return;
      }

      signinMsg.style.color = 'green';
      signinMsg.textContent = `Welcome, ${username}! | خوش آمدید، ${username}۔`;
      signinForm.reset();
    });

    // Sell فارم
    const sellForm = document.getElementById('sell-form');
    const sellMsg = document.getElementById('sell-msg');

    sellForm.addEventListener('submit', e => {
      e.preventDefault();
      const crop = sellForm['crop-name'].value.trim();
      const qty = sellForm.quantity.value;
      const contact = sellForm.contact.value.trim();

Pen Editor Menu

User Menu
HTML
CSS
JS
Result
75 unsaved changes 

HTML Options
      sellMsg.textContent = `Your crop "${crop}" of quantity ${qty} quintals has been submitted. | آپ کی فصل جمع ہوگئی ہے۔`;
      sellForm.reset();
    });
  });
</script>
​
</body>
</html>

      if(!crop || !qty || !contact){
        sellMsg.style.color = 'red';
        sellMsg.textContent = 'Please fill all fields correctly | تمام خانے صحیح طریقے سے پر کریں۔';
        return;
      }
      sellMsg.style.color = 'green';
      sellMsg.textContent = `Your crop "${crop}" of quantity ${qty} quintals has been submitted. | آپ کی فصل جمع ہوگئی ہے۔`;
      sellForm.reset();
    });
  });
</script>

</body>
</html>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

/* Reset */
* {
  box-sizing: border-box;
}

body {
  font-family: 'Roboto', sans-serif;
  margin: 0; padding: 0;
  background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1470&q=80') no-repeat center center fixed;
  background-size: cover;
  color: #1b3a1a;
  min-height: 100vh;
}

header {
  background: rgba(46, 125, 50, 0.95);
  padding: 12px 20px;
  color: white;
  position: sticky;
  top: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 700;
  padding: 8px 14px;
  border-radius: 6px;
  transition: background-color 0.3s ease;
  cursor: pointer;
}

nav a.active,
nav a:hover {
  background-color: #a3d38a;
  color: #1b3a1a;
}

.welcome-text {
  font-weight: 700;
  font-size: 1.2rem;
  white-space: nowrap;
}

main {
  background: rgba(255, 255, 255, 0.95);
  max-width: 1100px;
  margin: 30px auto;
  border-radius: 12px;
  padding: 25px 30px;
  box-shadow: 0 0 18px rgba(46, 125, 50, 0.4);
  min-height: 70vh;
}

section {
  display: none;
}

section.active {
  display: block;
}

h1, h2, h3 {
  color: #2e7d32;
  text-shadow: 1px 1px 3px #8bc34a;
}

h1 {
  font-weight: 900;
  font-size: 2rem;
  margin-bottom: 15px;
}

h2 {
  text-align: center;
  font-weight: 900;
  margin-bottom: 25px;
}

/* Grid for cards */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
  gap: 25px;
}

.card {
  background: #f7fff7;
  border-radius: 12px;
  padding: 18px;
  box-shadow: 0 0 10px #a3d38a99;
  border: 1px solid #c1d9ac;
  text-align: center;
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 0 18px #6aa84fbb;
}

.card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 10px;
  margin-bottom: 12px;
}

.card h3 {
  margin-bottom: 8px;
  font-weight: 700;
}

.card p {
  font-weight: 600;
  color: #4d662d;
}

/* Video container */
.video-container {
  max-width: 700px;
  margin: 35px auto 0;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 0 20px #8bc34a99;
}

video {
  width: 100%;
  height: auto;
  display: block;
}

/* Sign In form */
.signin-form-container {
  max-width: 400px;
  background: #eaf5df;
  border: 2px solid #8bc34a;
  padding: 20px 25px;
  border-radius: 15px;
  box-shadow: 0 0 12px #6aa84fbb;
  margin: 0 auto 30px;
}

.signin-form-container h2 {
  margin-bottom: 18px;
  font-weight: 900;
}

form label {
  font-weight: 700;
  display: block;
  margin-bottom: 6px;
  color: #2e7d32;
}

form input {
  width: 100%;
  padding: 10px 12px;
  margin-bottom: 18px;
  border-radius: 10px;
  border: 1.7px solid #a3d38a;
  font-size: 1rem;
  outline-color: #6aa84f;
}

form button {
  background: #4caf50;
  border: none;
  color: white;
  font-weight: 700;
  font-size: 1.15rem;
  padding: 12px;
  border-radius: 10px;
  cursor: pointer;
  width: 100%;
  transition: background-color 0.3s ease;
}

form button:hover {
  background: #81c784;
}

.message {
  font-weight: 700;
  margin-top: 12px;
  text-align: center;
}

/* AI Feature list */
#ai ul {
  list-style: none;
  max-width: 700px;
  margin: 0 auto;
  padding: 0;
}

#ai ul li {
  background: #dcedc8;
  margin: 12px 0;
  padding: 12px 18px;
  border-left: 6px solid #8bc34a;
  font-weight: 600;
  font-size: 1.1rem;
  color: #33691e;
  border-radius: 6px;
  box-shadow: 1px 1px 4px #a3d38aaa;
}

/* Sell form */
#sell form {
  max-width: 450px;
  margin: 0 auto;
}

#sell label {
  font-weight: 700;
  color: #2e7d32;
  display: block;
  margin-bottom: 6px;
}

#sell input {
  width: 100%;
  padding: 10px 8px;
  border-radius: 8px;
  border: 1.5px solid #a3d38a;
  margin-bottom: 15px;
  font-size: 1rem;
  outline-color: #6aa84f;
}

#sell button {
  background: #4caf50;
  border: none;
  color: white;
  padding: 12px 20px;
  font-size: 1.15rem;
  font-weight: 700;
  border-radius: 8px;
  cursor: pointer;
  width: 100%;
  transition: background-color 0.3s ease;
}

#sell button:hover {
  background: #81c784;
}

/* About */
#about p {
  font-size: 1.1rem;
  max-width: 850px;
  margin: 0 auto;
  line-height: 1.7;
  color: #3a5d1a;
  font-weight: 600;
  text-align: justify;
}

/* Responsive */
@media (max-width: 700px) {
  nav {
    justify-content: center;
  }
  .welcome-text {
    font-size: 1rem;
    margin-top: 8px;
    flex-basis: 100%;
    text-align: center;
  }
}
// نیویگیشن لنکس اور سیکشنز کو کنٹرول کرنا
const navLinks = document.querySelectorAll('nav a');
const sections = document.querySelectorAll('main section');

navLinks.forEach(link => {
  link.addEventListener('click', (e) => {
    e.preventDefault();

    // Active کلاس ہٹائیں تمام لنکس سے
    navLinks.forEach(l => l.classList.remove('active'));

    // کلک کیے گئے لنک پر active لگائیں
    link.classList.add('active');

    // جو سیکشن دکھانا ہے وہ نکالیں
    const target = link.getAttribute('data-section');

    // تمام سیکشنز چھپائیں
    sections.forEach(sec => sec.classList.remove('active'));

    // اگر target ملا تو اسے دکھائیں
    const targetSection = document.getElementById(target);
    if(targetSection) {
      targetSection.classList.add('active');
      targetSection.focus();
    }
  });
});

// Sign In فارم کا سبمٹ ایونٹ ہینڈل کریں
const signinForm = document.getElementById('signin-form');
const signinMsg = document.getElementById('signin-msg');

signinForm.addEventListener('submit', function(e) {
  e.preventDefault();

  const username = signinForm.username.value.trim();
  const password = signinForm.password.value.trim();

  if(username === '' || password === '') {
    signinMsg.style.color = 'red';
    signinMsg.textContent = 'Please enter both username and password | براہ کرم دونوں خانے پر کریں۔';
    return;
  }

  // یہاں لاگ ان کی اپنی ویلیڈیشن یا API کال کر سکتے ہیں
  signinMsg.style.color = 'green';
  signinMsg.textContent = `Welcome, ${username}! | خوش آمدید، ${username}۔`;

  signinForm.reset();
});
