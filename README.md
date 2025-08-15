# Jane-sales-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jane Lockhart Design - Luxury Personalized Interiors</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            overflow-x: hidden;
        }
        
        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #2c2c2c;
            background: #fefefe;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .hero {
            background: linear-gradient(135deg, #f8f6f3 0%, #ede7e0 100%);
            padding: 4rem 0;
            text-align: center;
            min-height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
        }
        
        .preheader {
            font-size: 0.95rem;
            color: #8b7d6b;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 1rem;
            font-weight: 500;
        }
        
        .main-headline {
            font-size: 3.5rem;
            font-weight: 300;
            color: #1a1a1a;
            margin-bottom: 1.5rem;
            line-height: 1.2;
            letter-spacing: -1px;
        }
        
        .subheader {
            font-size: 1.4rem;
            color: #5a5a5a;
            margin-bottom: 3rem;
            font-weight: 300;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .vsl-container {
            margin: 3rem 0;
            cursor: pointer;
        }
        
        .vsl-icon {
            position: relative;
            width: 300px;
            height: 200px;
            background: linear-gradient(45deg, #8b7d6b, #a69587);
            border-radius: 15px;
            margin: 0 auto 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 15px 40px rgba(139, 125, 107, 0.3);
            transition: transform 0.3s ease;
        }
        
        .vsl-icon:hover {
            transform: scale(1.05);
        }
        
        .play-button {
            width: 80px;
            height: 80px;
            background: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 8px 25px rgba(0,0,0,0.2);
        }
        
        .play-triangle {
            width: 0;
            height: 0;
            border-left: 25px solid #8b7d6b;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 8px;
        }
        
        .vsl-text {
            font-size: 1.1rem;
            color: #1a1a1a;
            font-weight: 500;
        }
        
        .primary-cta {
            background: #8b7d6b;
            color: white;
            padding: 18px 40px;
            font-size: 1.2rem;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            font-weight: 600;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            margin-top: 2rem;
            text-transform: uppercase;
        }
        
        .primary-cta:hover {
            background: #6d6152;
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(139, 125, 107, 0.4);
        }
        
        .section {
            padding: 5rem 0;
        }
        
        .section-headline {
            font-size: 2.8rem;
            font-weight: 300;
            text-align: center;
            margin-bottom: 3rem;
            color: #1a1a1a;
            line-height: 1.3;
        }
        
        .content-block {
            max-width: 900px;
            margin: 0 auto 2rem;
            text-align: center;
        }
        
        .content-block p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            color: #4a4a4a;
            line-height: 1.8;
        }
        
        .pain-point {
            background: #fff8f5;
            padding: 2rem;
            border-left: 5px solid #d4af8c;
            margin: 2rem 0;
            font-style: italic;
            font-size: 1.2rem;
        }
        
        .highlight {
            background: linear-gradient(120deg, #ffeaa7 0%, #fab1a0 100%);
            padding: 0.2em 0.5em;
            border-radius: 3px;
        }
        
        .bullet-list {
            text-align: left;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .bullet-item {
            background: white;
            padding: 2rem;
            margin: 1.5rem 0;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
            border-left: 4px solid #8b7d6b;
        }
        
        .bullet-item h3 {
            color: #8b7d6b;
            margin-bottom: 1rem;
            font-size: 1.4rem;
        }
        
        .two-column {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
            margin: 3rem 0;
        }
        
        .image-placeholder {
            background: linear-gradient(135deg, #f1f2f6, #ddd6fe);
            height: 400px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #666;
            font-size: 1.1rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .testimonial {
            background: white;
            padding: 2.5rem;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.08);
            margin: 2rem 0;
            text-align: center;
            border-top: 4px solid #8b7d6b;
        }
        
        .testimonial-text {
            font-size: 1.3rem;
            font-style: italic;
            color: #4a4a4a;
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: #8b7d6b;
            font-size: 1.1rem;
        }
        
        .faq-item {
            background: white;
            padding: 2rem;
            margin: 1.5rem 0;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
        }
        
        .faq-question {
            font-size: 1.3rem;
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 1rem;
        }
        
        .faq-answer {
            font-size: 1.1rem;
            color: #5a5a5a;
            line-height: 1.7;
        }
        
        .urgency-box {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            margin: 3rem 0;
        }
        
        .urgency-text {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }
        
        @media (max-width: 1024px) {
            .main-headline {
                font-size: 2.8rem;
            }
            .two-column {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            .container {
                padding: 0 1.5rem;
            }
        }
        
        @media (max-width: 768px) {
            .hero {
                padding: 2rem 0;
            }
            .main-headline {
                font-size: 2.2rem;
            }
            .subheader {
                font-size: 1.2rem;
            }
            .section-headline {
                font-size: 2.2rem;
            }
            .content-block p {
                font-size: 1.1rem;
            }
            .vsl-icon {
                width: 250px;
                height: 150px;
            }
            .container {
                padding: 0 1rem;
            }
            .section {
                padding: 3rem 0;
            }
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="preheader">For Affluent Homeowners & Executives</div>
            
            <h1 class="main-headline">Turn Your Home Into A Luxury Masterpiece That Commands Respect</h1>
            
            <p class="subheader">Without the stress of managing contractors, the overwhelm of endless decisions, or the fear of costly design mistakes that scream "amateur hour"</p>
            
            <div class="vsl-container">
                <a href="https://docs.google.com/document/d/1QKoUXPZZBRxbpR2r__uSRfKgBPz9rDLt71zFPYDPZBI/edit?usp=sharing" target="_blank">
                    <div class="vsl-icon">
                        <div class="play-button">
                            <div class="play-triangle"></div>
                        </div>
                    </div>
                    <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                </a>
            </div>
            
            <a href="#offer" class="primary-cta">Claim Your Design Consultation</a>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="section">
        <div class="container">
            <h2 class="section-headline">The Nightmare Every Successful Professional Faces When They Finally Decide To Upgrade Their Space...</h2>
            
            <div class="content-block">
                <p>You've worked your tail off.</p>
                
                <p>Built a successful business. Climbed the corporate ladder. Made the money.</p>
                
                <p>But every time you walk into your home... something feels <em>off</em>.</p>
                
                <div class="pain-point">
                    "This place should reflect my success, not look like I hired my cousin's friend who 'has good taste.'"
                </div>
                
                <p>You've tried the big box stores. Hired that designer your neighbor recommended. Spent weekends scrolling Pinterest until your eyes bled.</p>
                
                <p>Yet your home still feels like everyone else's...</p>
                
                <p>Generic. Cookie-cutter. <strong>Forgettable</strong>.</p>
                
                <p>And now when clients visit, or you host that dinner party, instead of feeling proud... you feel embarrassed.</p>
                
                <p>Because your space doesn't match your status.</p>
                
                <p>There IS a way to get the luxury, personalized space you deserve... without the headaches, without the regrets, and without looking like you tried too hard.</p>
            </div>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="section" style="background: #f9f7f4;">
        <div class="container">
            <h2 class="section-headline">How A Simple Realization Changed Everything About Luxury Interior Design</h2>
            
            <div class="two-column">
                <div>
                    <div class="image-placeholder">Award-winning designer Jane Lockhart in her Toronto studio</div>
                </div>
                <div class="content-block">
                    <p>Twenty-five years ago, Jane Lockhart had a problem.</p>
                    
                    <p>Her wealthy clients kept coming to her with the same frustration:</p>
                    
                    <p><em>"I can afford anything I want... so why does my home feel so ordinary?"</em></p>
                    
                    <p>That's when Jane realized something the entire industry had backwards...</p>
                    
                    <p>Most designers start with trends, not the person.</p>
                    
                    <p>They push what's "hot" instead of what fits your life, your personality, your success story.</p>
                    
                    <p>Jane developed what she calls the <span class="highlight">"Lifestyle-First Design Method"</span> — where every decision starts with understanding who you are and how you live.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="section">
        <div class="container">
            <h2 class="section-headline">The "Lifestyle-First Design Method" That Creates Spaces As Unique As Your Fingerprint</h2>
            
            <div class="content-block">
                <p>Here's how it works...</p>
                
                <p>Instead of showing you what's trendy, Jane starts by studying <em>you</em>.</p>
                
                <p>How you entertain. Where you unwind. What makes you feel most confident.</p>
                
                <p>Then she weaves those insights into every choice — from the texture of your wall coverings to the way light hits your dining table.</p>
            </div>
            
            <div class="bullet-list">
                <div class="bullet-item">
                    <h3>Deep Lifestyle Analysis</h3>
                    <p>So your space works with your daily rhythms instead of fighting against them, making every room feel like it was designed specifically for your life.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>Custom-Made Furniture Integration</h3>
                    <p>So you own pieces no one else has, making you the person whose home everyone remembers and talks about.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>Trend-Forward But Timeless Approach</h3>
                    <p>So your investment grows in value while staying ahead of the curve, positioning you as someone with impeccable taste who doesn't follow — they lead.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>White-Glove Project Management</h3>
                    <p>So you wake up one day to your dream space without dealing with contractor drama, making you the person who "has it all figured out."</p>
                </div>
            </div>
            
            <div class="testimonial">
                <div class="testimonial-text">"Our Blue Mountain home went from nice vacation property to the place everyone begs to visit. Jane didn't just design our space — she designed our reputation."</div>
                <div class="testimonial-author">— Executive Client, Blue Mountain Project</div>
            </div>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="section" style="background: #f9f7f4;">
        <div class="container">
            <h2 class="section-headline">Introducing: The Jane Lockhart Design Experience</h2>
            
            <div class="two-column">
                <div class="content-block">
                    <p>This isn't just interior design.</p>
                    
                    <p>This is a complete lifestyle elevation.</p>
                    
                    <p>While other designers give you variations of the same showroom looks...</p>
                    
                    <p>Jane creates spaces that feel authentically, unmistakably <em>yours</em>.</p>
                    
                    <p>The kind of home that makes people stop mid-conversation when they walk in.</p>
                    
                    <p>The kind that gets featured in magazines (like Jane's work regularly does).</p>
                    
                    <p>The kind that makes other successful people ask, <em>"Who did your design?"</em></p>
                </div>
                <div>
                    <div class="image-placeholder">Before/After luxury home transformation showcase</div>
                </div>
            </div>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="section" id="offer">
        <div class="container">
            <h2 class="section-headline">Here's Everything You Get When You Work With Jane Lockhart Design</h2>
            
            <div class="bullet-list">
                <div class="bullet-item">
                    <h3>✓ Personal Design Consultation & Vision Mapping</h3>
                    <p>Where Jane personally studies your lifestyle, preferences, and goals to create a design blueprint that fits your life like a custom suit, so you feel understood instead of sold to.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>✓ Access To Jane's Exclusive Made-In-Canada Furniture Line</h3>
                    <p>So you own pieces that literally cannot be found anywhere else, making you the person with the most enviable and unique style in your circle.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>✓ 2025 Trend Integration (Textured Whites, Vintage Accents, Warm Hues)</h3>
                    <p>So your home stays ahead of the curve without looking like you're trying too hard, positioning you as someone with natural sophistication.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>✓ Complete Project Management & Vendor Coordination</h3>
                    <p>So you avoid the nightmare of dealing with contractors and delays, making you the person who gets things done efficiently while others struggle.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>✓ Award-Winning Designer Credibility (Two-Time NKBA Pinnacle Award Winner)</h3>
                    <p>So when people ask about your designer, you can name-drop someone with real recognition, elevating your own status by association.</p>
                </div>
                
                <div class="bullet-item">
                    <h3>✓ Media-Featured Portfolio & TV Show Presence</h3>
                    <p>So you're working with someone who's appeared on HGTV and The Marilyn Denis Show, giving you confidence you're getting proven, recognized expertise.</p>
                </div>
            </div>
            
            <div class="urgency-box">
                <div class="urgency-text">Jane Only Takes On 12 New Projects Per Year</div>
                <p>Due to the intensive, personalized nature of her work, Jane can only accept a limited number of clients to maintain her standards of excellence.</p>
            </div>
            
            <div class="content-block" style="text-align: center;">
                <a href="#contact" class="primary-cta">Book Your Private Consultation</a>
                <p style="margin-top: 1rem; font-style: italic;">Investment details provided during consultation based on project scope</p>
            </div>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="section" style="background: #f9f7f4;">
        <div class="container">
            <h2 class="section-headline">Questions Successful People Ask Before Investing In Their Space</h2>
            
            <div class="faq-item">
                <div class="faq-question">Q: "I've been burned by designers before. How do I know Jane won't disappoint?"</div>
                <div class="faq-answer">Jane's 25 years of experience and two NKBA Pinnacle Awards speak louder than promises. Plus, her collaborative approach means your vision stays at the center of every decision. You're not gambling on unknown talent — you're investing in proven excellence.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: "I'm busy running my business. Will this consume all my time?"</div>
                <div class="faq-answer">That's exactly why Jane's concierge approach exists. You'll have input on the big decisions, but Jane's team handles all the coordination, vendor management, and project oversight. Most clients are amazed how little of their time is actually required.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: "What if my taste changes or I'm not happy with the direction?"</div>
                <div class="faq-answer">Jane's process includes multiple checkpoints and approvals before any major investments are made. Her collaborative approach means you see everything before it's implemented. This isn't about imposing her style — it's about perfecting yours.</div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: "How long does the process actually take?"</div>
                <div class="faq-answer">Most luxury projects are completed within 90 days from design approval to final installation. Jane's proven systems and established vendor relationships mean no delays, no surprises, just results on schedule.</div>
            </div>
            
            <div class="content-block" style="text-align: center; margin-top: 3rem;">
                <a href="#contact" class="primary-cta">Claim Your Consultation Before Spots Fill</a>
            </div>
        </div>
    </section>

    <!-- FINAL CONTACT -->
    <section class="section" id="contact" style="background: linear-gradient(135deg, #8b7d6b, #a69587); color: white;">
        <div class="container">
            <div class="content-block" style="text-align: center;">
                <h2 style="color: white; font-size: 2.5rem; margin-bottom: 2rem;">Your Dream Space Is One Decision Away</h2>
                
                <p style="font-size: 1.4rem; margin-bottom: 2rem;">Stop settling for ordinary when you've earned extraordinary.</p>
                
                <p style="font-size: 1.2rem; margin-bottom: 3rem;">Book your private consultation with Jane Lockhart and start living in a space that matches your success.</p>
                
                <a href="mailto:info@janelockhart.com" class="primary-cta" style="background: white; color: #8b7d6b;">Get Started Today</a>
                
                <p style="margin-top: 2rem; font-size: 0.9rem; opacity: 0.8;">Limited availability • Serious inquiries only</p>
            </div>
        </div>
    </section>
</body>
</html>
