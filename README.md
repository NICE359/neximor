<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NEXIMOR Limited</title>

<style>
body{
    margin:0;
    font-family:Segoe UI, Arial, sans-serif;
    background:#f4f6f8;
    color:#333;
}
header{
    background:linear-gradient(135deg,#0a1f44,#12326b);
    color:#fff;
    padding:50px 20px;
    text-align:center;
}
header h1{margin:0;font-size:34px;}
header p{margin-top:10px;font-size:16px;opacity:.9}

section{
    max-width:1100px;
    margin:auto;
    padding:50px 20px;
}
h2{color:#0a1f44;margin-bottom:20px}

.services,.gallery{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.card{
    background:#fff;
    padding:25px;
    border-radius:10px;
    box-shadow:0 6px 15px rgba(0,0,0,.1);
}
.card h3{color:#0a1f44;margin-top:0}
.card p{font-size:14.5px;line-height:1.6}

.btn{
    display:inline-block;
    margin-top:15px;
    padding:12px 18px;
    background:#0a1f44;
    color:#fff;
    text-decoration:none;
    border-radius:6px;
    font-size:14px;
    font-weight:600;
}
.btn:hover{background:#12326b}

.gallery div{
    height:160px;
    background:#ddd;
    border-radius:8px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:600;
    color:#555;
}

form input,form select,form textarea{
    width:100%;
    padding:12px;
    margin-bottom:15px;
    border-radius:6px;
    border:1px solid #ccc;
}

footer{
    background:#0a1f44;
    color:#fff;
    text-align:center;
    padding:25px 15px;
    font-size:14px;
}
</style>
</head>

<body>

<header>
<h1>NEXIMOR Limited</h1>
<p>Engineering • Energy • Construction • Smart Technology Solutions</p>
</header>

<section>
<h2>About Us</h2>
<p>
NEXIMOR Limited is a multidisciplinary engineering, construction, and smart
technology company delivering safe, reliable, and innovative solutions.
We specialize in turbine services, smart systems, and building works.
</p>
</section>

<section>
<h2>Our Goods & Services</h2>

<div class="services">

<div class="card">
<h3>Smart Lock Installation</h3>
<p>Supply, installation, and configuration of fingerprint, card, PIN, and mobile smart locks.</p>
<a class="btn" href="https://wa.me/2348114154073?text=I%20need%20Smart%20Lock%20Installation">Request Service</a>
</div>

<div class="card">
<h3>Turbine Pre-Commissioning</h3>
<p>Inspection, loop checks, calibration, and system readiness verification.</p>
<a class="btn" href="https://wa.me/2348114154073?text=I%20need%20Turbine%20Pre-Commissioning">Request Service</a>
</div>

<div class="card">
<h3>Turbine Commissioning</h3>
<p>Safe start-up, testing, performance validation, and handover.</p>
<a class="btn" href="https://wa.me/2348114154073?text=I%20need%20Turbine%20Commissioning">Request Service</a>
</div>

<div class="card">
<h3>House Building</h3>
<p>Residential and commercial building construction from foundation to completion.</p>
<a class="btn" href="https://wa.me/2348114154073?text=I%20need%20House%20Building">Request Service</a>
</div>

<div class="card">
<h3>Painting & Finishing</h3>
<p>Interior & exterior painting, renovation, and finishing works.</p>
<a class="btn" href="https://wa.me/2348114154073?text=I%20need%20Painting%20Service">Request Service</a>
</div>

</div>
</section>

<section>
<h2>Request a Service / Get a Quote</h2>

<form onsubmit="sendToWhatsApp();return false;">
<input id="name" placeholder="Full Name" required>
<input id="phone" placeholder="Phone Number" required>
<select id="service" required>
<option value="">Select Service</option>
<option>Smart Lock Installation</option>
<option>Turbine Pre-Commissioning</option>
<option>Turbine Commissioning</option>
<option>House Building</option>
<option>Painting & Finishing</option>
</select>
<textarea id="message" rows="4" placeholder="Additional details"></textarea>
<button class="btn" type="submit">Submit Request</button>
</form>
</section>

<section>
<h2>Project Gallery</h2>
<div class="gallery">
<div>Smart Lock Project</div>
<div>Turbine Site Work</div>
<div>Building Construction</div>
<div>Painting Project</div>
</div>
</section>

<section>
<h2>Online Payment</h2>
<p>
Online payment is available for confirmed jobs and supplies.
Click below to proceed with payment after receiving your quotation.
</p>
<a class="btn" href="#">Pay Now (Paystack Enabled)</a>
</section>

<section>
<h2>Contact Us</h2>
<p>
📧 Email: info@neximor.com <br>
📞 Phone / WhatsApp: +234 811 415 4073
</p>
</section>

<footer>
<p>© 2025 NEXIMOR Limited. All Rights Reserved.</p>
</footer>

<script>
function sendToWhatsApp(){
var n=document.getElementById("name").value;
var p=document.getElementById("phone").value;
var s=document.getElementById("service").value;
var m=document.getElementById("message").value;

var url="https://wa.me/2348114154073?text="
+"Hello%20NEXIMOR%0A"
+"Name:%20"+encodeURIComponent(n)+"%0A"
+"Phone:%20"+encodeURIComponent(p)+"%0A"
+"Service:%20"+encodeURIComponent(s)+"%0A"
+"Details:%20"+encodeURIComponent(m);

window.open(url,"_blank");
}
</script>

</body>
</html>
