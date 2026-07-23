<!DOCTYPE html>
<html lang="en">
<head>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600;700&family=Pacifico&display=swap" rel="stylesheet">
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SpringKids Family Daycare </title>
  <link rel="stylesheet" href="style1.css" />
</head>
<body>

<header class="navbar">
  <div class="logo-icon">
  <img src="logoheader.png" alt="SpringKids Logo">
</div>
    <div>
      <h1>SpringKids</h1>
      <p>FAMILY DAYCARE</p>
    </div>
  </div>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About Us</a>
    <a href="#programs">Programs</a>
    <a href="#gallery">Gallery</a>
    <a href="#enrollment">Enrollment</a>
    <a href="#contact">Contact</a>
  </nav>
  <div class="navbar-right">
  <a href="#contact" class="tour-btn">Schedule a Tour</a>
  <div id="google_translate_element"></div>
</header>

<section id="home" class="hero">
  <div class="hero-text">
    <p class="welcome">🌿 Welcome to</p>
    <h2><span>SpringKids</span><br>Family Daycare</h2>
    <h3>Learn • Play • Grow</h3>
    <p>A warm, caring environment where children feel safe, loved, and inspired every day.</p>

    <div class="hero-buttons">
      <a href="#contact" class="btn">Schedule a Tour</a>
      
      <a href="#enrollment" class="btn-outline">Join Waitlist</a>
    </div>
  </div>
  <div class="hero-image">
    <img src="background.png" alt="SpringKids Family Daycare">
  </div>
</section>

<section class="why-us">
  <h2>🌿 Why Families Choose Us 🌿</h2>
  <div class="features">
    <div><div class="icon">🏠</div><h3>Licensed</h3><p>Licensed Family Daycare</p></div>
    <div><div class="icon">💬</div><h3>Bilingual</h3><p>English & Chinese Support</p></div>
    <div><div class="icon">🍎</div><h3>Healthy Meals</h3><p>Nutritious Daily Meals</p></div>
    <div><div class="icon">👧</div><h3>Small Group</h3><p>Low Child-to-Caregiver Ratio</p></div>
    <div><div class="icon">🛡️</div><h3>Safe & Loving</h3><p>Nurturing and Secure Environment</p></div>
  </div>
</section>

<section id="about" class="section">
  <h2>About Us</h2>
  <p>
    SpringKids Family Daycare LLC provides a safe, loving, and home-like environment
    for children to learn, play, and grow. We support each child’s social, emotional,
    and early learning development through daily routines, creative play, and caring guidance.
  </p>
</section>

<section id="programs" class="section light">
  <h2>Our Programs</h2>
  <div class="cards">
    <div class="card"><h3>Infants</h3><p>Gentle care, feeding, naps, music, and safe play.</p></div>
    <div class="card"><h3>Toddlers</h3><p>Story time, movement, art, sensory play, and social skills.</p></div>
    <div class="card"><h3>Preschool</h3><p>Letters, numbers, creativity, routines, and school readiness.</p></div>
  </div>
</section>
<section id="gallery" class="section">
  <h2>Gallery</h2>

  <div class="gallery-grid">

    <div class="gallery-card">
      <p>Play Area</p>
    </div>

    <div class="gallery-card">

      <div class="gallery-card">

  <p>Healthy Meals</p>

  <div class="photo-slider">
    <button class="arrow left-arrow" onclick="prevMeal()">❮</button>

    <img id="mealPhoto"
         src="FOOD1.png"
         alt="Healthy Meals"
         class="gallery-photo">

    <button class="arrow right-arrow" onclick="nextMeal()">❯</button>
  </div>

</div>

  <p>Learning Time</p>

  <div class="photo-slider">
    <button class="arrow left-arrow" onclick="prevPhoto()">❮</button>

    <img id="learningPhoto"
         src="learning-time2.png"
         alt="Learning Time"
         class="gallery-photo">

    <button class="arrow right-arrow" onclick="nextPhoto()">❯</button>
  </div>

</div>

    <div class="gallery-card">
      <p>Art Activities</p>
    </div>

  </div>
</section>
<section id="enrollment" class="section light">
  <h2>Enrollment</h2>
  <p>
    We welcome families to contact us for availability, program details, and enrollment information.
    Please reach out to schedule a tour or join our waitlist.
  </p>
    <button class="btn" onclick="openForm()">
    Request Information
  </button>
 <!-- <div id="enrollmentPopup" class="popup">
    <div class="popup-content">
      <span class="close" onclick="closeForm()">&times;</span>

      <h2>Enrollment Inquiry</h2>

      <form class="enrollment-form">
        <label>Child's Name</label>
        <input type="text" placeholder="Enter child's name">

        <label>Child's Age</label>
        <input type="number" placeholder="Enter child's age">

        <label>Gender</label>
        <select>
          <option>Select Gender</option>
          <option>Female</option>
          <option>Male</option>
          <option>Prefer Not to Say</option>
        </select>

        <label>Parent / Guardian Name</label>
        <input type="text" placeholder="Enter parent name">

        <label>Phone Number</label>
        <input type="tel" placeholder="Enter phone number">

        <label>Email Address</label>
        <input type="email" placeholder="Enter email address">

        <button type="submit" class="btn">Submit Inquiry</button>
      </form>
    </div>
  </div>
</section>

</section>-->

<section id="contact" class="section contact">
  <h2>Contact Us</h2>

  <p>
    <strong>Email:</strong>
    <a href="mailto:your@email.com">hrspringkids@gmail.com</a>
  </p>

  <div class="wechat-section">
    <h3>WeChat</h3>

    <img src="wechat-qrcode.png"
         alt="WeChat QR Code"
         class="wechat-qrcode">

    <p>Scan the QR code to contact us.</p>
  </div>

</section>

<footer>
  <p>© 2026 SpringKids Family Daycare LLC. All Rights Reserved.</p>
</footer>
<script>
const photos = [
  "learning-time2.png",
  "learning-time1.png"
];

let currentPhoto = 0;

function nextPhoto() {
  currentPhoto = (currentPhoto + 1) % photos.length;
  document.getElementById("learningPhoto").src = photos[currentPhoto];
}

function prevPhoto() {
  currentPhoto = (currentPhoto - 1 + photos.length) % photos.length;
  document.getElementById("learningPhoto").src = photos[currentPhoto];
}
</script>
  <script>
const mealPhotos = [
  "FOOD1.png",
  "food2.JPG",
  "food3.JPG"
];

let currentMeal = 0;

function nextMeal() {
  currentMeal = (currentMeal + 1) % mealPhotos.length;
  document.getElementById("mealPhoto").src = mealPhotos[currentMeal];
}

function prevMeal() {
  currentMeal = (currentMeal - 1 + mealPhotos.length) % mealPhotos.length;
  document.getElementById("mealPhoto").src = mealPhotos[currentMeal];
}
</script>
  <script>
function googleTranslateElementInit() {
  new google.translate.TranslateElement(
    {
      pageLanguage: 'en',
      includedLanguages: 'en,zh-CN,es',
      layout: google.translate.TranslateElement.InlineLayout.SIMPLE
    },
    'google_translate_element'
  );
}
</script>

<script src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
<!--<script>
function openForm() {
  document.getElementById("enrollmentPopup").style.display = "block";
}

function closeForm() {
  document.getElementById("enrollmentPopup").style.display = "none";
}
</script>-->
</body>
</html>
