<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AgriBridge - Instant Payouts & Logistics</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap" rel="stylesheet">
    <link rel="icon" href="https://via.placeholder.com/32?text=AB" type="image/png"> <!-- Favicon placeholder; replace with your logo -->
    <style>
        body { 
            font-family: 'Open Sans', sans-serif; 
            margin: 0; 
            padding: 0; 
            background: #F8F8F8; 
            color: #333; 
            line-height: 1.6; 
            overflow-x: hidden; /* Prevent horizontal scroll */
        }
        header { 
            background: linear-gradient(to right, rgb(34, 151, 180), rgb(204, 204, 204)); 
            color: rgb(5, 0, 0); 
            text-align: center; 
            padding: 120px 20px 80px; 
            position: relative;
        }
        h1 { 
            font-size: clamp(2em, 5vw, 3em); /* Responsive font size */
            margin: 0 0 10px 0; 
        }
        header p { 
            font-size: clamp(1em, 3vw, 1.2em); 
            max-width: 600px; 
            margin: 0 auto 20px; 
        }
        .cta { 
            background: #058019; 
            color: white; 
            padding: 15px 30px; 
            border: none; 
            font-size: clamp(1em, 2.5vw, 1.2em); 
            cursor: pointer; 
            border-radius: 5px; 
            transition: background 0.3s ease; /* Smooth hover */
            min-height: 50px; /* Touch-friendly */
            display: inline-block;
        }
        .cta:hover { background: #E55A2B; }
        section { 
            padding: 60px 20px; 
            max-width: 1200px; 
            margin: 0 auto; 
        }
        .features { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 
            gap: 30px; 
        }
        .features h2 { 
            text-align: center; 
            grid-column: 1 / -1; 
            font-size: clamp(1.5em, 4vw, 2em); 
        }
        .card { 
            background: white; 
            padding: 30px 20px; /* More padding for touch */
            border-radius: 8px; 
            box-shadow: 0 2px 10px rgba(0,0,0,0.1); 
            text-align: center; 
            transition: transform 0.3s ease; /* Hover lift */
        }
        .card:hover { transform: translateY(-5px); }
        .card h3 { 
            color: #228B22; 
            margin-bottom: 10px; 
        }
        #form section { 
            background: #F8F8F8; /* Subtle bg for form section */
        }
        .form-container {
            max-width: 640px;
            margin: 0 auto;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .form-iframe {
            width: 100%;
            height: 797px;
            border: none;
            border-radius: 5px;
        }
        footer { 
            background: #333; 
            color: white; 
            text-align: center; 
            padding: 30px 20px; 
            font-size: 0.9em;
        }
        /* Enhanced Mobile Media Queries */
        @media (max-width: 768px) { 
            header { 
                padding: 80px 15px 60px; /* Reduced for small screens */
            }
            .features { 
                grid-template-columns: 1fr; /* Stack cards on mobile */
                gap: 20px; 
                padding: 0 10px;
            }
            .card { 
                padding: 25px 15px; 
            }
            .form-container { 
                padding: 15px;
                margin: 0 10px;
            }
            .form-iframe {
                height: 600px; /* Shorter on mobile for better fit */
            }
            section { 
                padding: 40px 15px; /* Less padding on sides */
            }
        }
        @media (max-width: 480px) { 
            h1 { font-size: 1.8em; }
            .cta { 
                padding: 18px 25px; 
                min-height: 55px; /* Even larger touch target */
            }
            .form-iframe {
                height: 500px; /* Even shorter for tiny screens */
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>AgriBridge</h1>
        <p>Instant ZMW payouts + cold chain logistics for Zambian farmers & SMBs. Export without the hassle.</p>
        <button class="cta" onclick="document.getElementById('form').scrollIntoView({behavior: 'smooth'});">Join Waitlist</button>
    </header>
    
    <section class="features">
        <h2>Why AgriBridge?</h2>
        <div class="card">
            <h3>Fast Payouts</h3>
            <p>USD to MTN/Airtel in seconds—no delays.</p>
        </div>
        <div class="card">
            <h3>Cold Chain</h3>
            <p>Keep your produce fresh from farm to buyer.</p>
        </div>
        <div class="card">
            <h3>Low Fees</h3>
            <p>1-2% only—save on every export.</p>
        </div>
        <div class="card">
            <h3>One-Stop Hub</h3>
            <p>Payments + shipping, all in one app.</p>
        </div>
    </section>
    
    <section id="form">
        <h2 style="text-align: center;">Get Early Access</h2>
        <div class="form-container">
            <iframe class="form-iframe" src="https://docs.google.com/forms/d/e/1FAIpQLSe-q5G778A6yTFkc1G1VWR2xBBSjpOYLQ6rILJKbMbNLiEqmg/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
        </div>
    </section>
    
    <footer>
        <p>&copy; 2025 AgriBridge | Built in Zambia | Contact: hello@agrib ridge.zm</p>
    </footer>
</body>
</html>
