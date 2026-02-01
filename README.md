
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1"/>

  <title> Zameer Travels Madanapalle| Madanapalle to Andhra Pradesh</title>
  <marquee style="color:blue;font-size: 40px;font-style: calc();"> Zameer Travels Madanapalle</marquee>

  <meta name="description" content="Zameer travels MAdanapalle and across Andhra Pradesh. Trusted by 1000+ customers.">
  <meta name="keywords" content="Hyderabad airport taxi, Bangalore airport cabs, outstation cabs Andhra Pradesh">
  <meta name="author" content="Zameer Travels ">

  <link rel="stylesheet" href="style.css" />

  <!-- ✅ iOS Premium UI styles only for booking hero (safe, doesn't break existing styles) -->
  <style>
    /* iOS Premium background */
    .ios-bg {
      position: absolute;
      inset: 0;
      overflow: hidden;
      z-index: 0;
      border-radius: 22px;
      pointer-events: none;
    }
    .ios-bg .blob {
      position: absolute;
      width: 320px;
      height: 320px;
      border-radius: 50%;
      filter: blur(45px);
      opacity: 0.55;
      transform: translate3d(0,0,0);
    }
    .ios-bg .blob-1 { top:-120px; left:-90px; background: #01ffaa; }
    .ios-bg .blob-2 { bottom:-150px; right:-120px; background: #4dff68; }
    .ios-bg .blob-3 { top:20%; right:-160px; background: #34ffa4; opacity:.38; }

    .booking-hero {
      position: relative;
      overflow: hidden;
      border-radius: 24px;
      padding: 16px;
      background: rgba(255,255,255,0.12);
      backdrop-filter: blur(18px);
      -webkit-backdrop-filter: blur(18px);
      border: 1px solid rgba(255,255,255,0.24);
      box-shadow: 0 18px 60px rgba(0,0,0,0.25);
      z-index: 1;
    }

    /* premium tab buttons */
    .booking-tabs {
      display: flex;
      gap: 10px;
      background: rgba(255,255,255,0.12);
      padding: 10px;
      border-radius: 18px;
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      border: 1px solid rgba(255,255,255,0.18);
      position: relative;
      z-index: 2;
    }
    .booking-tabs .tab {
      flex: 1;
      border-radius: 14px;
      font-weight: 800;
      padding: 12px 12px;
      border: none;
      cursor: pointer;
      transition: 0.2s ease;
      background: transparent;
      color: #111;
    }
    .booking-tabs .tab.active {
      background: linear-gradient(135deg, #ffd24a, #f7b500);
      box-shadow: 0 10px 26px rgba(212, 179, 14, 0.864);
      transform: translateY(-1px);
    }

    /* booking card like iPhone glass */
    .booking-card {
      margin-top: 14px;
      padding: 16px;
      border-radius: 22px;
      background: rgba(255,255,255,0.16);
      backdrop-filter: blur(18px);
      -webkit-backdrop-filter: blur(18px);
      border: 1px solid rgba(255,255,255,0.22);
      box-shadow: 0 18px 60px rgba(0,0,0,0.22);
      position: relative;
      z-index: 2;
    }

    /* segmented control for local/outstation */
    .segmented {
      display: flex;
      gap: 10px;
      padding: 10px;
      border-radius: 18px;
      background: rgba(0,0,0,0.08);
      margin: 12px 0 12px;
    }
    .seg-btn {
      flex: 1;
      padding: 12px;
      border: none;
      border-radius: 14px;
      font-weight: 900;
      cursor: pointer;
      background: transparent;
      transition: 0.2s;
    }
    .seg-btn.active {
      background: linear-gradient(135deg,#cac228, #ffff00);
      color: #111;
      box-shadow: 0 10px 25px rgba(247,181,0,0.25);
    }

    /* iOS inputs inside local booking */
    #localBooking label {
      font-weight: 700;
    }
    #localBooking input,
    #localBooking select {
      border-radius: 14px;
      padding: 14px;
      border: 1px solid rgba(0,0,0,0.10);
      background: rgba(255,255,255,0.85);
      outline: none;
    }
    #localBooking input:focus,
    #localBooking select:focus {
      border-color: rgba(247, 181, 0, 0.993);
      box-shadow: 0 0 0 4px rgb(230, 169, 3);
    }
    .seg-form { display: none; }
    .seg-form.active { display: block; }

    .ios-primary-btn {
      width: 100%;
      padding: 14px;
      border-radius: 16px;
      border: none;
      cursor: pointer;
      font-weight: 900;
      background: linear-gradient(135deg, #ffd24a, #f7b500);
      box-shadow: 0 14px 34px rgba(247,181,0,0.25);
    }
  </style>
</head>

<body>

<!-- HEADER -->
<header class="header">
  <div class="logo">ZAMEER TRAVELS <span>MADANAPALLE</span></div>
  <nav>
    <a href="#airport">Airport Cabs</a>
    <a href="#services">Services</a>
    <a href="#about">About</a>
    <a href="#contact" class="btn">Book Now</a>
  </nav>
</header>

<!-- HERO -->
<section id="airport" class="hero">
  <h1>Reliable Airport Cabs from Bangalore to Madanapalle</h1>
  <p>Safe • On-time • Transparent Pricing • Trusted by 10,00+ customers</p>

  <section id="booking-hero" class="booking-hero">
    <!-- iOS premium blobs -->
    <div class="ios-bg">
      <div class="blob blob-1"></div>
      <div class="blob blob-2"></div>
      <div class="blob blob-3"></div>
    </div>

    <!-- TABS -->
    <div class="booking-tabs">
      <button class="tab active" onclick="showBooking('airport')">Airport Ride</button>
      <button class="tab" onclick="showBooking('local')">Local / Outstation</button>
      <button class="tab" onclick="showBooking('acting driver')">acting  driver</button>
    </div>

    <div class="booking-card">

      <!-- ✅ LOCAL / OUTSTATION (NEW, iOS UI) -->
      <div id="localBooking" class="booking-form">
        <div class="steps">
          <span class="active">1 Search</span>
          <span>2 Choose</span>
          <span>3 Pay</span>
        </div>

        <!-- segmented -->
        <div class="segmented">
          <button id="segOutstation" class="seg-btn active" onclick="switchSeg('outstation')">
            🛣️ Outstation
          </button>
          <button id="segLocal" class="seg-btn" onclick="switchSeg('local')">
            🚕 Local
          </button>
        </div>

        <!-- OUTSTATION FORM -->
        <div id="outstationForm" class="seg-form active">
          <label>Leaving From</label>
          <input id="out_from" list="city_list" placeholder="Eg: Madanapalle" />

          <label>Going To</label>
          <input id="out_to" list="city_list" placeholder="Eg: Bangalore" />

          <label>Date</label>
          <input type="date" id="out_date" />

          <button class="ios-primary-btn" onclick="startOutstationSearch()">
            🔍 Search Outstation Rides
          </button>
        </div>

        <!-- LOCAL FORM -->
        <div id="localForm" class="seg-form">
          <label>City</label>
          <input id="loc_city" placeholder="Eg: Madanapalle" value="Madanapalle" />

          <label>Area (Optional)</label>
          <input id="loc_area" placeholder="Eg: Bangalore / Airport" />

          <button class="ios-primary-btn" onclick="startLocalSearch()">
            🔍 Search Local Rides
          </button>
        </div>

        <!-- city list -->
        <datalist id="city_list">
          <option>Madanapalle</option>
          <option>Bangalore</option>
          <option>chittoor</option>
          <option>kadapa</option>
          <option>piler</option>
          <option>Tirupati</option>
          <option>Nellore</option>
          <option>Kurnool</option>
          <option>mysuru</option>
          <option>vellore</option>
        </datalist>
      </div>

      <!-- ✅ AIRPORT BOOKING (UNCHANGED IDs + logic) -->
      <div id="airportBooking" class="booking-form active">

        <div class="steps">
          <span class="active">1 Location</span>
          <span>2 Contact</span>
          <span>3 Review</span>
        </div>

        <!-- STEP 1 -->
        <div class="step step-1 active">

          <div class="radio-group">
            <label><input type="radio" name="tripType" value="From Airport" checked onchange="handleTripTypeChange()"> From Airport</label>
            <label><input type="radio" name="tripType" value="To Airport" onchange="handleTripTypeChange()"> To Airport</label>
          </div>

          <label>Pickup</label>
          <select id="pickup_airport">
            <option value="">Select Airport</option>
            <option>kempagouda International Airport</option>
            <option>Tirupati International Airport</option>
            <option>Kadapa Airport</option>
            <option>chennai International Airport</option>
          </select>

          <input id="pickup_manual" style="display:none" placeholder="Enter pickup location">

          <label>Drop</label>
          <input id="drop_manual" list="drop_routes" placeholder="Enter drop location">
          <datalist id="drop_routes"></datalist>

          <label>Date</label>
          <input type="date" id="date">

          <label>Time</label>
          <input type="time" id="time">

          <button onclick="validateStep1()">Continue</button>
        </div>

        <!-- STEP 2 -->
        <div class="step step-2">
          <label>Name</label>
          <input id="name">

          <label>Phone</label>
          <input id="phone">

          <button onclick="validateStep2()">Continue</button>
        </div>

        <!-- STEP 3 -->
        <div class="step step-3">
          <div id="review"></div>

          <button id="finalActionBtn" class="whatsapp-btn">
            Continue
          </button>
        </div>

      </div>

      <div id="airportResults"></div>
    </div>

    <!-- ACTING  DRIVER -->
    <div id="ActingDriveBooking" class="booking-form">
      <h2>Drivers</h2>
      <p>Choose from a wide range of Acting-drive cars in Madanapalle.</p>

      <h3>Experienced Drivers 9381581773</h3>
    </div>

  </section>
</section>

<!-- WHY ZAMEER TRAVELS MADANAPALLE -->
<section class="why-Zameer Travels Madanapalle">
  <div class="container">
    <h2>Why Choose <span>Zameer Travels</span>?</h2>

    <div class="why-grid">
      <div class="why-card">
        <div class="icon">✈️</div>
        <h3>Airport Specialists</h3>
        <p>Dedicated airport cab services with punctual pickups & drops your safety is our main Priority.</p>
      </div>

      <div class="why-card">
        <div class="icon">🛡️</div>
        <h3>Verified Drivers</h3>
        <p>Background-checked, trained drivers for safe journeys we care about yourself.</p>
      </div>

      <div class="why-card">
        <div class="icon">💰</div>
        <h3>No Hidden Charges</h3>
        <p>Transparent pricing with zero last-minute surprises and reasonable prices.</p>
      </div>

      <div class="why-card">
        <div class="icon">📞</div>
        <h3>24/7 Support</h3>
        <p>Always-on customer support before, during & after your ride.</p>
      </div>
    </div>
  </div>
</section>

<!-- SERVICES -->
<div class="services-grid">


  <!-- Airport -->
 <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTS3_OOL9Bbz2mbOCf3giqES8M0SfFo3oZY1w&s " alt="Photo" style="width:350px" >
        
      <h3>Airport Transfers</h3>
      <p>On-time pickups & drops with professional drivers.</p>
      <div class="price">From ₹3500</div>
      <div class="service-actions">
        <a href="#booking" class="btn small">Book Now</a>
        <a href="https://wa.me/919381581773" class="btn ghost">WhatsApp</a>
      </div>
    </div>
  </div>

  <!-- Outstation -->
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSeopBlk0Sqo47yEPOc3agA0ui86qrb7z6RAg&s" alt="Photo" style="width:400px" >
      <h3>Outstation Trips</h3>
      <p>Comfortable long-distance travel at transparent prices.</p>
      <div class="price">From ₹12/km</div>
      <div class="service-actions">
        <a href="#booking" class="btn small">Book Now</a>
        <a href="https://wa.me/919381581773" class="btn ghost">WhatsApp</a>
      </div>
    </div>
  </div>

  <!-- Corporate -->
  <img src="https://sushmatravels.com/wp-content/uploads/2026/01/Tempo-Traveller-rent-1024x683.png" alt="Photo" style="width:400px" >
      <h3>Corporate Travel</h3>
      <p>Reliable transport for teams & executives.</p>
      <div class="price">Custom Plans</div>
      <div class="service-actions">
        <a href="#contact" class="btn small">Enquire</a>
      </div>
    </div>
  </div>

  <!-- Rentals -->
  <div class="service-card smart-rentals reveal">
    <span class="badge">Coming Soon</span>
    <div class="overlay"></div>
    <div class="service-content center">
      <div class="service-icon big">🚘</div>
      <h3>Smart Rentals</h3>
      <p>driver & long-term rentals with flexible plans.</p>
    </div>
  </div>

</div>

<!-- VEHICLES -->
<section class="vehicle-options">
  <div class="section-heading">
    <span class="tagline">Choose Your Ride</span>
    <h2>Vehicle Options</h2>
    <p>Comfortable rides for every journey</p>
  </div>

  <div class="vehicle-grid">

    <!-- SEDAN -->
    <div class="vehicle-card">
      <div class="vehicle-icon">🚗</div>
      <h3>Sedan</h3>
      <p class="models">Dzire / Etios</p>

      <div class="features">
        <span>👤 4 Seater</span>
        <span>🧳 2 Bags</span>
        <span class="ac">❄ AC</span>
      </div>

      <div class="price">From ₹12/km</div>

      <a href="https://wa.me/919381581773?text=Hi%20Taxigo,%20I%20want%20to%20book%20a%20Sedan%20from%20Airport"
         target="_blank"
         class="vehicle-btn">
        Book Now
      </a>
    </div>

    <!-- SUV -->
    <div class="vehicle-card">
      <div class="vehicle-icon">🚙</div>
      <h3>SUV</h3>
      <p class="models">Innova</p>

      <div class="features">
        <span>👤 6 Seater</span>
        <span>🧳 4 Bags</span>
        <span class="ac">❄ AC</span>
      </div>

      <div class="price">From ₹16/km</div>

      <a href="https://wa.me/919381581773?text=Hi%20Taxigo,%20I%20want%20to%20book%20a%20Sedan%20from%20Airport"
         target="_blank"
         class="vehicle-btn">
        Book Now
      </a>
    </div>

    <!-- TEMPO TRAVELLER-->
    <div class="vehicle-card premium">
      <span class="badge">TEMPO</span>
      <div class="vehicle-icon">✨</div>
      <h3>Premium</h3>
      <p class="models">TEMPO TRAVELLER</p>

      <div class="features">
        <span>👤 14 Seater</span>
        <span>🧳 10 Bags</span>
        <span class="ac">❄ AC</span>
      </div>

      <div class="price">From ₹25/km</div>

      <a href="https://wa.me/9381581773?text=Hi%20Taxigo,%20I%20want%20to%20book%20a%20Sedan%20from%20Airport"
         target="_blank"
         class="vehicle-btn">
        Book Now
      </a>
    </div>

  </div>
</section>

<!-- SOCIAL PROOF -->
<section class="trust-section">
  <div class="container">
    <h2 class="trust-title">Trusted by Thousands</h2>

    <div class="trust-cards">
      <div class="trust-card">
        <h3>100+ Trips</h3>
        <p>Successfully completed airport rides</p>
      </div>

      <div class="trust-card">
        <h3>10K+ Followers</h3>
        <p>Growing community across platforms</p>
      </div>

      <div class="trust-card">
        <h3>500K+ Reach</h3>
        <p>Monthly audience & brand visibility</p>
      </div>
    </div>
  </div>
</section>

<!-- OUR STORY SECTION -->
<section class="journey">
  <h2 class="section-title">Our Journey</h2>
  <p class="section-subtitle">
    From the driver’s seat to building a trusted travel brand
  </p>

  <div class="timeline">
    <div class="timeline-item fade-scroll">
      <div class="icon">🚕</div>
      <div class="content">
        <h4>Learning the Roads</h4>
        <p>
          Started as a professional driver at a travel company, gaining
          hands-on experience in airport and outstation operations.
        </p>
      </div>
    </div>

    <div class="timeline-item fade-scroll">
      <div class="icon">🚀</div>
      <div class="content">
        <h4>2000 – Birth of Travels</h4>
        <p>
          Founded <strong>ZAMEER TRAVELS MADANAPALLE/strong> with a clear focus on reliable
          airport transfers and customer-first service.
        </p>
      </div>
    </div>

    <div class="timeline-item fade-scroll">
      <div class="icon">⭐</div>
      <div class="content">
        <h4>100+ Trips Milestone</h4>
        <p>
          Completed 100+ trips within months and built strong trust with
          regular customers.
        </p>
      </div>
    </div>

    <div class="timeline-item fade-scroll">
      <div class="icon">📍</div>
      <div class="content">
        <h4>Growing Across Cities</h4>
        <p>
          Expanding services from Madanapalle to Bangalore & Hyderabad with
          airport transfers and upcoming Smart Rentals.
        </p>
      </div>
    </div>
  </div>
</section>

<!-- TESTIMONIALS -->
<section class="testimonials">
  <div class="container">
    <h2>What Our Customers Say</h2>

    <div class="testimonial-grid">
      <div class="testimonial-card">
        <p>“Very punctual and clean car. Smooth airport drop.”</p>
        <span>KARTHIK KUMAR - MADANAPALLE</span>
      </div>

      <div class="testimonial-card">
        <p>“Professional driver and transparent pricing.”</p>
        <span>— PRAVEEN, AMERICA</span>
      </div>

      <div class="testimonial-card">
        <p>“Best experience for outstation travel.”</p>
        <span>— NARMADA, Tirupati</span>
      </div>
    </div>
  </div>
</section>

<!-- FOUNDER SECTION -->
<section class="founder-profile">
  <div class="container founder-flex">

    <div class="founder-img">
      <img src="C:\Users\zameerdell\Pictures\zameerpic.jpeg"
           alt="P Syed Zameer – Founder of Zameer Travels Madanapalle">
    </div>

    <div class="founder-text">
      <h2>Meet the Founder</h2>
      <h3>P SYED ZAMEER</h3>
      <span>Founder & Operations Head</span>

      <p>
        Zameer founded this with a clear mission — to build a dependable,
        customer-first travel brand rooted in real operational experience.
      </p>

      <p class="quote">
        “Every ride should feel reliable, comfortable, and worth the customer’s trust.”
      </p>
    </div>

  </div>
</section>

<!-- FOOTER -->
<footer>
  <p>©️ 2025 Travels Rides | Safe • Reliable • Affordable</p>
</footer>

<a href="https://wa.me/919381581773"
   class="whatsapp-float"
   target="_blank">
   💬
</a>

<script>
  const RATE = {
    sedan: 12,
    suv: 15,
    premium: 18
  };

  function calculatePrice(type, km) {
    return km * RATE[type];
  }
</script>

<script>
  const scrollElements = document.querySelectorAll(".fade-scroll");

  const elementInView = (el, offset = 100) => {
    const elementTop = el.getBoundingClientRect().top;
    return elementTop <= window.innerHeight - offset;
  };

  const displayScrollElement = (element) => {
    element.classList.add("show");
  };

  const handleScrollAnimation = () => {
    scrollElements.forEach((el) => {
      if (elementInView(el)) {
        displayScrollElement(el);
      }
    });
  };

  window.addEventListener("scroll", handleScrollAnimation);
</script>

<script src="script.js"></script>
</body>
<script>'undefined'=== typeof _trfq || (window._trfq = []);'undefined'=== typeof _trfd && (window._trfd=[]),_trfd.push({'tccl.baseHost':'secureserver.net'},{'ap':'cpsh-oh'},{'server':'sg2plzcpnl508403'},{'dcenter':'sg2'},{'cp_id':'10832508'},{'cp_cl':'8'}) // Monitoring performance to make your website faster. If you want to opt-out, please contact web hosting support.</script><script src='https://img1.wsimg.com/traffic-assets/js/tccl.min.js'></script></html>


