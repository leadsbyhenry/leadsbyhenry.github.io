# leadsbyhenry.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leads by Henry</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

<header>
    <div class="container">
        <img src="images/logo.png" alt="Leads by Henry Logo" class="logo">
        <h1>Leads by Henry</h1>
        <p>10–20 New Clients Every Month for Your Gym or Coaching Business</p>
        <a href="#signup" class="cta-button">Get Started</a>
    </div>
</header>

<section class="how-it-works">
    <div class="container">
        <h2>How It Works</h2>
        <p>We generate high-quality leads for your business using Instagram, TikTok, and simple online tools. You only pay if results are delivered. No risk, just clients.</p>
    </div>
</section>

<section class="pricing">
    <div class="container">
        <h2>Pricing</h2>
        <div class="price-box">
            <p><strong>First Month:</strong> $1,500 for 10–20 qualified leads</p>
            <p><strong>Ongoing:</strong> $1,500/month</p>
            <a href="#signup" class="cta-button">Claim Your Leads</a>
        </div>
    </div>
</section>

<section id="signup" class="signup">
    <div class="container">
        <h2>Sign Up / Contact</h2>
        <p>Fill out the form below and start getting new clients immediately!</p>
        <!-- Embed Google Form -->
        <iframe src="YOUR_GOOGLE_FORM_LINK_HERE" width="100%" height="800" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    </div>
</section>

<footer>
    <div class="container">
        <p>&copy; 2025 Leads by Henry. All rights reserved.</p>
    </div>
</footer>

</body>
</html>
/* General */
body {
    font-family: 'Roboto', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #ffffff;
    color: #333;
}

.container {
    max-width: 900px;
    margin: auto;
    padding: 0 20px;
}

/* Header */
header {
    background-color: #ffffff;
    text-align: center;
    padding: 60px 20px;
    border-bottom: 1px solid #eee;
}

header h1 {
    margin: 20px 0 10px;
    font-size: 2.5em;
    color: #222;
}

header p {
    font-size: 1.2em;
    color: #555;
}

.logo {
    max-width: 150px;
    margin-bottom: 20px;
}

.cta-button {
    display: inline-block;
    background-color: #00A86B;
    color: white;
    padding: 15px 30px;
    text-decoration: none;
    font-weight: bold;
    border-radius: 8px;
    margin-top: 20px;
    transition: 0.3s;
}

.cta-button:hover {
    background-color: #007f55;
}

/* Sections */
section {
    padding: 60px 0;
}

section h2 {
    text-align: center;
    font-size: 2em;
    margin-bottom: 20px;
}

section p {
    text-align: center;
    font-size: 1.1em;
    max-width: 700px;
    margin: 0 auto;
}

/* Pricing */
.pricing .price-box {
    text-align: center;
    background-color: #f9f9f9;
    padding: 40px 20px;
    border-radius: 10px;
    margin-top: 20px;
    box-shadow: 0px 5px 15px rgba(0,0,0,0.05);
}

/* Footer */
footer {
    background-color: #f5f5f5;
    text-align: center;
    padding: 30px 20px;
    border-top: 1px solid #eee;
    color: #555;
}

/* Responsive */
@media(max-width: 600px) {
    header h1 {
        font-size: 2em;
    }
    section h2 {
        font-size: 1.5em;
    }
    .cta-button {
        padding: 12px 25px;
    }
}

