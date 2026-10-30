

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ujb</title>
    <!-- clean, professional fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600&family=Playfair+Display:wght@500;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
		
       body {
		    background: url('tree.jpg') center center / cover no-repeat fixed;
		    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
		    color: #1e2b3c;
		    line-height: 1.6;
		    min-height: 100vh;
		    display: flex;
		    align-items: center;
		    justify-content: center;
		    padding: 2rem 1.5rem;
}
		
        .container {
            max-width: 820px;
            width: 100%;
            background: #CAE0D5;
            border-radius: 24px;
            box-shadow: 0 4px 24px rgba(0, 0, 0, 0.04), 0 1px 2px rgba(0, 0, 0, 0.02);
            padding: 3rem 3.5rem;
            border: 2px solid #FF0A30;
            transition: box-shadow 0.3s ease;
        }
		
        .container:hover {
            box-shadow: 0 80px 40px rgba(0, 0, 0, 0.06);
        }
		
        /* header area */
        .header {
            display: flex;
            align-items: center;
            gap: 2rem;
            margin-bottom: 2.5rem;
            flex-wrap: wrap;
        }
		
        .avatar {
            width: 96px;
            height: 96px;
            border-radius: 50%;
            background: #e8edf3;
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Playfair Display', serif;
            font-size: 2.6rem;
            font-weight: 600;
            color: #2c3e50;
            flex-shrink: 0;
            border: 3px solid #ffffff;
            box-shadow: 0 2px 12px rgba(0, 0, 0, 0.06);
            letter-spacing: -1px;
        }
		
        .title h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
            font-weight: 600;
            color: #1a2632;
            line-height: 1.2;
            letter-spacing: -0.01em;
        }
		
        .title .subtitle {
            font-size: 1rem;
            font-weight: 400;
            color: #6b7c8f;
            margin-top: 0.3rem;
            letter-spacing: 0.3px;
        }

        .title .subtitle span {
            color: #3b5e7d;
            font-weight: 500;
        }

        /* subtle divider */
        .divider {
            height: 1px;
            background: linear-gradient(90deg, #eef2f6, #d0dae6, #eef2f6);
            margin: 1.8rem 0 2rem;
        }

        /* welcome line — simple & warm */
        .welcome {
            font-size: 1.15rem;
            font-weight: 400;
            color: #3e4f62;
            margin-bottom: 2rem;
            padding-left: 0.2rem;
            border-left: 3px solid #b0c4d9;
            padding-left: 1rem;
            background: #f8fafc;
            border-radius: 0 12px 12px 0;
            padding: 0.7rem 1.2rem;
            font-style: italic;
            letter-spacing: 0.2px;
        }

        /* info cards — modest grid */
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 1.2rem;
            margin-bottom: 2.2rem;
        }


        .info-item {
            background: #f9fbfd;
            border-radius: 16px;
            padding: 1.2rem 1.4rem;
            border: 1px solid #eef2f6;
            transition: border-color 0.2s ease, background 0.2s ease;
        }

        .info-item:hover {
            border-color: #000000;
            background: #ffffff;
        }

        .info-item h3 {
            font-size: 0.75rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1.2px;
            color: #6b7c8f;
            margin-bottom: 0.6rem;
        }

        .info-item p {
            font-size: 1rem;
            font-weight: 400;
            color: #253544;
            line-height: 1.5;
        }

        .info-item p strong {
            font-weight: 600;
            color: #1a2632;
        }
         /* ── NEW: Education section ── */
        .education {
            margin-top: 2.5rem;
        }

        .education h2 {
            font-family: 'Playfair Display', serif;
            font-size: 1.3rem;
            font-weight: 600;
            color: #1a2632;
            margin-bottom: 1.2rem;
            letter-spacing: -0.01em;
        }

        .edu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 1.2rem;
        }

        .edu-item {
            background: #f9fbfd;
            border-radius: 16px;
            padding: 1.3rem 1.4rem;
            border: 1px solid #eef2f6;
            border-left: 3px solid #b0c4d9;
            transition: border-color 0.2s ease, background 0.2s ease, border-left-color 0.2s ease;
        }

        .edu-item:hover {
            background: #ffffff;
            border-color: #cbd9e8;
            border-left-color: #4b6a88;
        }

        .edu-item h4 {
            font-size: 1rem;
            font-weight: 600;
            color: #1a2632;
            margin-bottom: 0.35rem;
            line-height: 1.4;
        }

        .edu-item .institution {
            font-size: 0.9rem;
            font-weight: 500;
            color: #4b6a88;
            margin-bottom: 0.35rem;
        }

        .edu-item .edu-meta {
            font-size: 0.85rem;
            font-weight: 400;
            color: #6b7c8f;
            font-style: italic;
        }


        /* bio block */
        .bio {
            display: flex;
            flex-wrap: wrap;
            gap: 1.8rem;
            align-items: flex-end;
            margin-top: 1rem;
        }

        .bio-text {
            flex: 2;
            min-width: 240px;
            font-size: 1rem;
            color: #3e4f62;
            line-height: 1.7;
        }

        .bio-text .highlight {
            font-weight: 500;
            color: #1e3b5a;
            background: #eef4fa;
            padding: 0.1rem 0.3rem;
            border-radius: 6px;
        }

        .signature {
            flex: 1;
            min-width: 120px;
            text-align: right;
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            font-weight: 500;
            color: #6b7c8f;
            letter-spacing: 1px;
            border-right: 2px solid #d0dae6;
            padding-right: 1rem;
            align-self: flex-end;
            opacity: 0.85;
        }

        /* links row — clean & minimal */
        .links {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            margin-top: 2.5rem;
            padding-top: 1.5rem;
            border-top: 1px solid #eef2f6;
            justify-content: flex-end;
        }

        .links a {
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 500;
            color: #4b6a88;
            letter-spacing: 0.3px;
            transition: color 0.2s ease, transform 0.15s ease;
            display: inline-flex;
            align-items: center;
            gap: 6px;
            padding-bottom: 2px;
            border-bottom: 1px solid transparent;
        }

        .links a:hover {
            color: #1e3b5a;
            border-bottom-color: #b0c4d9;
        }

        .links a .arrow {
            font-size: 1rem;
            color: #9bb0c4;
            transition: transform 0.2s ease, color 0.2s ease;
        }

        .links a:hover .arrow {
            transform: translateX(3px);
            color: #4b6a88;
        }

        /* responsive */
        @media (max-width: 640px) {
            .container {
                padding: 2rem 1.8rem;
                border-radius: 20px;
            }
            .header {
                gap: 1.2rem;
            }
            .avatar {
                width: 72px;
                height: 72px;
                font-size: 2rem;
            }
            .title h1 {
                font-size: 1.8rem;
            }
            .welcome {
                font-size: 1rem;
            }
            .signature {
                text-align: left;
                border-right: none;
                border-left: 2px solid #d0dae6;
                padding-left: 1rem;
                padding-right: 0;
                margin-top: 0.8rem;
            }
            .links {
                justify-content: flex-start;
                gap: 1.5rem;
            }
        }

        @media (max-width: 420px) {
            .container {
                padding: 1.8rem 1.2rem;
            }
            .info-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- header with avatar + name -->
        <div class="header">
            <div class="avatar">HS</div>
            <div class="title">
                <h1>Heta SUTO</h1>
                <div class="subtitle"> Mathematics Teacher | Data Manager | Aspiring Data Engineer <span>·</span> Systems Thinker</div>
            </div>
        </div>

        <!-- welcome line (originally from the <p> tag) -->
        <div class="welcome">
            Welcome to my webpage..
        </div>

        <!-- modest info grid: quick facts -->
        <div class="info-grid">
            <div class="info-item">
                <h3>based in</h3>
                <p><strong>Goroka</strong><br>Eastern Highlands Province</p>
            </div>
            <div class="info-item">
                <h3>focus</h3>
                <p>Data Engineering, <strong>ETL Data Pipelines</strong>, Data Management.</p>
            </div>
            <div class="info-item">
                <h3>tools</h3>
                <p>R Studio · Python · STATA <strong> · REDCap </strong> · MS Excel</p>
            </div>
            <div class="info-item">
                <h3>Interest</h3>
                <p><strong>I Have many interest </strong><br>open to conversations</p>
            </div>

                <div class="info-item">
                <h3>Educational Background</h3>
                <p>Bachelor of Mathematics and Computer Science <strong> DWU</strong> · PostGraduate Diploma in STEM Education <strong> UOG</strong> </p>
            </div>
            <div class="info-item">
                <h3>contact</h3>
                <p><strong>hetasuto924@gmail.com </strong><br>open to conversations</p>
            </div>
        </div>

        <!-- subtle divider -->
        <div class="divider"></div>

        <!-- bio paragraph + signature -->
        <div class="bio">
            <div class="bio-text">
                Whatever the mind of man can <span class="highlight">CONCEIVE</span>
                He can <span class="highlight">ACHIEVE</span>. 
            </div>
            <div class="signature">Napolean Hill</div>
        </div>

        <!-- ── NEW: Education section ── -->
        <div class="divider"></div>

         <div class="education">
            <h2>Education</h2>
            <div class="edu-grid">
                <div class="edu-item">
                    <h4>Postgraduate Diploma in STEM Education</h4>
                    <div class="institution">University of Goroka (UOG)</div>
                    <div class="edu-meta">Focus on integrative STEM pedagogy and curriculum design</div>
                </div>
                <div class="edu-item">
                    <h4>Bachelor of Mathematics &amp; Computing Science</h4>
                    <div class="institution">Divine Word University (DWU)</div>
                    <div class="edu-meta">Foundations in mathematical reasoning, algorithms, and software systems</div>
                </div>
            </div>
        </div>

        <!-- clean social links -->
<div class="links">
    <a href="https://www.linkedin.com/in/heta-suto-655203229/" target="_blank" rel="noopener noreferrer">
        <span class="arrow">→</span> LinkedIn
    </a>
    <a href="mailto:hetasuto924@gmail.com">
        <span class="arrow">→</span> Email
    </a>
</div>
    </div>

</body>
</html>
