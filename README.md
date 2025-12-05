<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>KS DIGITAL SERVICES</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
/* Reset and Base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-tap-highlight-color: transparent;
}

body {
  font-family: 'Inter', sans-serif;
  background: #ffffff;
  color: #333333;
  line-height: 1.4;
  min-height: 100vh;
  padding: 15px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Main Container */
.container {
  max-width: 500px;
  margin: 0 auto;
  background: #ffffff;
  border-radius: 12px;
  overflow: hidden;
}

/* Title - Minimal Gap */
.title-section {
  text-align: center;
  margin-bottom: 10px;
}

h1 {
  font-family: 'Poppins', sans-serif;
  font-size: 24px;
  font-weight: 700;
  color: #2c3e50;
  margin-bottom: 5px;
  padding-bottom: 8px;
  border-bottom: 2px solid #3498db;
}

/* Main Page Button - Very Small Gap */
.main-page-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: #27ae60;
  color: white;
  padding: 10px 20px;
  border-radius: 25px;
  text-decoration: none;
  font-weight: 500;
  font-size: 14px;
  margin: 0;
  transition: all 0.2s;
  width: auto;
  max-width: 180px;
}

.main-page-btn:hover {
  background: #219653;
  transform: scale(1.02);
}

/* SINGLE LINE BUTTONS - All 3 in one row */
.contact-buttons-single-row {
  display: flex;
  gap: 8px;
  margin: 15px 0 20px 0;
  justify-content: space-between;
  width: 100%;
  flex-wrap: nowrap; /* Prevent wrapping */
}

/* Each button in the row */
.single-btn {
  flex: 1;
  min-width: 0; /* Allow buttons to shrink */
  background: white;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 12px 8px;
  text-decoration: none;
  color: #333;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  transition: all 0.2s;
  box-shadow: 0 2px 5px rgba(0,0,0,0.05);
  text-align: center;
}

.single-btn:active {
  transform: scale(0.98);
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

.btn-icon-small {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  color: white;
  margin-bottom: 6px;
}

.btn-text {
  font-size: 11px;
  font-weight: 600;
  color: #2c3e50;
  line-height: 1.2;
  word-wrap: break-word;
}

.btn-subtext {
  font-size: 10px;
  color: #666;
  margin-top: 2px;
}

/* Button colors */
.call-btn .btn-icon-small { background: #27ae60; }
.maps-btn .btn-icon-small { background: #3498db; }
.whatsapp-btn .btn-icon-small { background: #25D366; }

/* Offerings List */
.offerings-section {
  margin: 20px 0;
}

.section-title {
  font-family: 'Poppins', sans-serif;
  font-size: 18px;
  font-weight: 600;
  color: #2c3e50;
  text-align: center;
  margin-bottom: 15px;
  padding-bottom: 5px;
  border-bottom: 1px solid #eee;
}

.offerings-list {
  list-style: none;
  display: grid;
  grid-template-columns: 1fr;
  gap: 8px;
}

.offerings-list li {
  padding: 10px 12px 10px 35px;
  background: #f8f9fa;
  border-radius: 6px;
  font-size: 14px;
  color: #444;
  position: relative;
  border-left: 3px solid #3498db;
}

.offerings-list li::before {
  content: '✓';
  position: absolute;
  left: 12px;
  color: #27ae60;
  font-weight: bold;
  font-size: 14px;
}

/* Contact Info */
.contact-info {
  background: #f8f9fa;
  border-radius: 10px;
  padding: 15px;
  margin: 20px 0;
  border-top: 2px solid #3498db;
}

.contact-info h3 {
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  color: #2c3e50;
  margin-bottom: 12px;
  text-align: center;
  font-weight: 600;
}

.contact-details {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 10px;
  color: #555;
  font-size: 14px;
}

.contact-item i {
  color: #3498db;
  width: 20px;
  font-size: 14px;
}

.phone-number {
  font-size: 15px;
  color: #2c3e50;
  font-weight: 600;
  margin-top: 5px;
}

/* Footer */
footer {
  text-align: center;
  padding: 15px;
  color: #666;
  font-size: 12px;
  background: #f8f9fa;
  border-radius: 8px;
  margin-top: 15px;
}

.footer-content p {
  margin-bottom: 5px;
}

.copyright {
  font-size: 11px;
  color: #888;
  margin-top: 8px;
}

/* Mobile-specific adjustments */
@media (max-width: 480px) {
  body {
    padding: 12px;
  }
  
  h1 {
    font-size: 22px;
  }
  
  .contact-buttons-single-row {
    gap: 6px;
    margin: 12px 0 18px 0;
  }
  
  .single-btn {
    padding: 10px 6px;
  }
  
  .btn-icon-small {
    width: 30px;
    height: 30px;
    font-size: 13px;
  }
  
  .btn-text {
    font-size: 10px;
  }
  
  .btn-subtext {
    font-size: 9px;
  }
  
  .offerings-list li {
    padding: 9px 10px 9px 32px;
    font-size: 13px;
  }
  
  .main-page-btn {
    padding: 9px 18px;
    font-size: 13px;
  }
}

@media (max-width: 350px) {
  h1 {
    font-size: 20px;
  }
  
  .contact-buttons-single-row {
    gap: 4px;
  }
  
  .single-btn {
    padding: 8px 4px;
  }
  
  .btn-text {
    font-size: 9px;
  }
  
  .btn-subtext {
    font-size: 8px;
  }
}

/* Ensure no horizontal scroll on mobile */
html, body {
  overflow-x: hidden;
  width: 100%;
}

/* Touch-friendly buttons */
button, a {
  cursor: pointer;
  -webkit-user-select: none;
  user-select: none;
}
</style>

</head>
<body>

<div class="container">
  <!-- 1. KS DIGITAL SERVICES Title -->
  <div class="title-section">
    <h1>KS DIGITAL SERVICES</h1>
    
    <!-- 2. Main Page Link Button - Minimal Gap -->
    <a class="main-page-btn" href="https://ksdigitalservice.pw/">
      <i class="fas fa-home"></i>
      Main Page
    </a>
  </div>
  
  <!-- 3. ALL 3 BUTTONS IN SINGLE LINE -->
  <div class="contact-buttons-single-row">
    <!-- Call Button -->
    <a class="single-btn call-btn" href="tel:+917893845696">
      <div class="btn-icon-small">
        <i class="fas fa-phone-alt"></i>
      </div>
      <div class="btn-text">Call Now</div>
      <div class="btn-subtext">7893845696</div>
    </a>
    
    <!-- Maps Button -->
    <a class="single-btn maps-btn" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank">
      <div class="btn-icon-small">
        <i class="fas fa-map-marker-alt"></i>
      </div>
      <div class="btn-text">Get Directions</div>
      <div class="btn-subtext">Location</div>
    </a>
    
    <!-- WhatsApp Button -->
    <a class="single-btn whatsapp-btn" href="https://wa.me/7893845696" target="_blank">
      <div class="btn-icon-small">
        <i class="fab fa-whatsapp"></i>
      </div>
      <div class="btn-text">WhatsApp</div>
      <div class="btn-subtext">Chat Now</div>
    </a>
  </div>
  
  <!-- 4. Offerings as a List -->
  <div class="offerings-section">
    <h2 class="section-title">Our Services & Offerings</h2>
    <ul class="offerings-list">
      <li>FSSAI / Trade / Labor License</li>
      <li>GST Registration / Returns</li>
      <li>ITR Filing (Income Tax)</li>
      <li>PF (EPFO) Services</li>
      <li>Passport / PAN Card / Voter ID</li>
      <li>AEPS Money Withdrawal</li>
      <li>Credit Card to Bank Transfer</li>
      <li>Aadhar Address Change</li>
      <li>Train / Bus / Flight Ticket Bookings</li>
      <li>All Entrance Exams Applications</li>
      <li>Insurance & Bank A/C Opening</li>
      <li>Plastic PVC Card Printing</li>
      <li>Project Works / Resume Making</li>
      <li>Document Editing</li>
      <li>Rental Agreement</li>
      <li>Scholarships Fresh / Renewal</li>
      <li>Tally ERP Services</li>
      <li>PM Vishwakarma, ABHA, PMEGP</li>
      <li>Senior Citizen (Aasara Card)</li>
      <li>DOST Application & TTD Bookings</li>
      <li>Property Tax / Electricity Bill Payment</li>
    </ul>
  </div>
  
  <!-- 5. Contact Info -->
  <div class="contact-info">
    <h3>Contact Information</h3>
    <div class="contact-details">
      <div class="contact-item">
        <i class="fas fa-clock"></i>
        <span>Business Hours: 7:00 AM - 10:00 PM</span>
      </div>
      <div class="contact-item">
        <i class="fas fa-envelope"></i>
        <span>Email: ksdigital2025@gmail.com</span>
      </div>
      <div class="contact-item phone-number">
        <i class="fas fa-phone"></i>
        <span>+91 78938 45696</span>
      </div>
    </div>
  </div>
</div>

<!-- 6. Footer -->
<footer>
  <div class="footer-content">
    <p>© 2025 KS Digital Services</p>
    <p>Providing reliable digital solutions</p>
    <p class="copyright">Designed for mobile users</p>
  </div>
</footer>

</body>
</html>
