<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avan Dodhia - Investment Banking Professional</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Crimson+Text:wght@400;600;700&family=Source+Serif+Pro:wght@400;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'dark-primary': '#0a0f1c',
                        'dark-secondary': '#1a2332',
                        'dark-accent': '#2a3441',
                        'gold-accent': '#d4af37',
                        'blue-accent': '#4a90e2',
                        'text-primary': '#e8eaed',
                        'text-secondary': '#9aa0a6',
                        'text-muted': '#5f6368'
                    },
                    fontFamily: {
                        'inter': ['Inter', 'sans-serif'],
                        'crimson': ['Crimson Text', 'serif'],
                        'source': ['Source Serif Pro', 'serif']
                    }
                }
            }
        }
    </script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.7;
            color: #e8eaed;
            background: #0a0f1c;
            overflow-x: hidden;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #0a0f1c 0%, #1a2332 50%, #2a3441 100%);
        }
        
        .section-gradient {
            background: linear-gradient(180deg, #1a2332 0%, #0a0f1c 100%);
        }
        
        .card-shadow {
            background: rgba(42, 52, 65, 0.6);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(212, 175, 55, 0.1);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            transition: all 0.4s ease;
        }
        
        .card-shadow:hover {
            background: rgba(42, 52, 65, 0.8);
            border: 1px solid rgba(212, 175, 55, 0.3);
            box-shadow: 0 16px 48px rgba(0, 0, 0, 0.4);
            transform: translateY(-8px);
        }
        
        .text-gradient {
            background: linear-gradient(135deg, #d4af37, #4a90e2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #d4af37, #b8941f);
            color: #0a0f1c;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            background: linear-gradient(135deg, #b8941f, #d4af37);
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(212, 175, 55, 0.4);
        }
        
        .btn-outline {
            border: 2px solid #d4af37;
            color: #d4af37;
            transition: all 0.3s ease;
        }
        
        .btn-outline:hover {
            background: #d4af37;
            color: #0a0f1c;
            transform: translateY(-3px);
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(40px);
            transition: all 1s ease;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .slide-in-left {
            opacity: 0;
            transform: translateX(-60px);
            transition: all 1s ease;
        }
        
        .slide-in-left.visible {
            opacity: 1;
            transform: translateX(0);
        }
        
        .slide-in-right {
            opacity: 0;
            transform: translateX(60px);
            transition: all 1s ease;
        }
        
        .slide-in-right.visible {
            opacity: 1;
            transform: translateX(0);
        }
        
        .progress-bar {
            width: 0%;
            transition: width 2.5s ease-in-out;
            background: linear-gradient(90deg, #d4af37, #4a90e2);
        }
        
        .nav-blur {
            backdrop-filter: blur(15px);
            background: rgba(10, 15, 28, 0.9);
            border-bottom: 1px solid rgba(212, 175, 55, 0.1);
        }
        
        .section-divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
        }
        
        .premium-text {
            font-family: 'Crimson Text', serif;
            font-weight: 600;
            letter-spacing: 0.5px;
        }
        
        .body-text {
            font-family: 'Source Serif Pro', serif;
            font-size: 1.1rem;
            line-height: 1.8;
            color: #9aa0a6;
        }
        
        .accent-glow {
            box-shadow: 0 0 20px rgba(212, 175, 55, 0.3);
        }
        
        @media (max-width: 768px) {
            .hero-text {
                font-size: 2.5rem;
            }
            .body-text {
                font-size: 1rem;
                line-height: 1.7;
            }
        }
    </style>
</head>
<body class="bg-dark-primary">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 nav-blur">
        <div class="max-w-7xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="font-crimson font-bold text-2xl text-gold-accent">
                    <img src="Avan.png>
                    Avan Dodhia
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#about" class="text-text-secondary hover:text-gold-accent transition-colors font-medium">About</a>
                    <a href="#experience" class="text-text-secondary hover:text-gold-accent transition-colors font-medium">Experience</a>
                    <a href="#certifications" class="text-text-secondary hover:text-gold-accent transition-colors font-medium">Certifications</a>
                    <a href="#expertise" class="text-text-secondary hover:text-gold-accent transition-colors font-medium">Expertise</a>
                    <a href="#contact" class="text-text-secondary hover:text-gold-accent transition-colors font-medium">Contact</a>
                </div>
                <button id="mobile-menu" class="md:hidden text-gold-accent">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="min-h-screen flex items-center justify-center hero-gradient pt-20">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <div class="fade-in">
                <h1 class="font-crimson font-bold text-6xl md:text-8xl mb-6 text-gradient hero-text">
                    Avan Dodhia
                </h1>
                <div class="text-2xl md:text-3xl text-gold-accent mb-8 font-medium premium-text">
                    Investment Banking Fellow • ACCA Professional
                </div>
                <p class="body-text mb-12 max-w-4xl mx-auto">
                    Currently advancing through the prestigious Marquee Fellowship Program while leveraging comprehensive 
                    audit expertise with NIFTY 50 companies. Specialized in M&A advisory, financial modeling, and capital 
                    markets with proven track record in ₹24,000+ crore revenue corporations and Goldman Sachs risk simulation certification.
                </p>
                <div class="flex flex-col sm:flex-row gap-6 justify-center">
                    <a href="#experience" class="btn-primary px-8 py-4 rounded-lg font-semibold text-lg">
                        View Experience
                    </a>
                    <a href="#contact" class="btn-outline px-8 py-4 rounded-lg font-semibold text-lg">
                        Connect With Me
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 section-gradient">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="font-crimson font-bold text-5xl mb-4 text-text-primary fade-in">
                    Professional Profile
                </h2>
                <div class="section-divider w-24 mx-auto mb-8"></div>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="slide-in-left">
                    <h3 class="font-crimson font-semibold text-3xl mb-6 text-gold-accent">
                        Investment Banking Excellence
                    </h3>
                    <div class="space-y-6 body-text">
                        <p>
                            Currently advancing through the prestigious <strong class="text-gold-accent">Marquee Fellowship Program</strong> 
                            while leveraging comprehensive audit experience with NIFTY 50 companies and ₹24,000+ crore revenue corporations. 
                            Deep expertise in financial analysis, due diligence, and valuation methodologies.
                        </p>
                        <p>
                            Proven track record in statutory audits, financial modeling, and regulatory compliance across 
                            pharmaceuticals and manufacturing sectors. <strong class="text-gold-accent">ACCA qualification (11/13 papers)</strong> 
                            combined with <strong class="text-gold-accent">Goldman Sachs Risk Simulation certification</strong> provides 
                            robust foundation in corporate finance and strategic analysis.
                        </p>
                        <p>
                            Specialized in M&A advisory, capital structure optimization, and financial risk assessment with 
                            hands-on experience in IPO preparation and due diligence processes. Active contributor to college 
                            cultural activities and beatboxing competitions, demonstrating well-rounded leadership capabilities.
                        </p>
                    </div>
                </div>
                
                <div class="slide-in-right">
                    <div class="grid grid-cols-2 gap-6">
                        <div class="card-shadow p-8 rounded-xl text-center accent-glow">
                            <div class="text-4xl font-bold text-gold-accent mb-2">₹24,500+</div>
                            <div class="text-text-secondary font-medium">Crores Audited</div>
                        </div>
                        <div class="card-shadow p-8 rounded-xl text-center">
                            <div class="text-4xl font-bold text-blue-accent mb-2">11/13</div>
                            <div class="text-text-secondary font-medium">ACCA Papers</div>
                        </div>
                        <div class="card-shadow p-8 rounded-xl text-center">
                            <div class="text-4xl font-bold text-gold-accent mb-2">35%</div>
                            <div class="text-text-secondary font-medium">Error Reduction</div>
                        </div>
                        <div class="card-shadow p-8 rounded-xl text-center">
                            <div class="text-4xl font-bold text-blue-accent mb-2">100%</div>
                            <div class="text-text-secondary font-medium">QA Compliance</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-20 bg-dark-primary">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="font-crimson font-bold text-5xl mb-4 text-text-primary fade-in">
                    Professional Experience
                </h2>
                <div class="section-divider w-24 mx-auto mb-8"></div>
            </div>
            
            <div class="space-y-12">
                <div class="card-shadow p-8 rounded-xl fade-in">
                    <div class="flex flex-col lg:flex-row lg:justify-between lg:items-start mb-6">
                        <div>
                            <h3 class="font-crimson font-semibold text-2xl mb-2 text-gold-accent">
                                Investment Banking Fellow
                            </h3>
                            <div class="text-xl text-blue-accent mb-2 premium-text">Marquee Fellowship Program</div>
                        </div>
                        <div class="text-text-secondary font-medium">July 2025 - Present</div>
                    </div>
                    <p class="body-text mb-6">
                        Currently advancing through prestigious investment banking fellowship program, developing expertise in 
                        M&A advisory, capital markets, and financial modeling. Gaining hands-on experience in deal structuring, 
                        valuation methodologies, and client relationship management within investment banking environment.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">M&A Advisory</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">Capital Markets</span>
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">Financial Modeling</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">Deal Structuring</span>
                    </div>
                </div>

                <div class="card-shadow p-8 rounded-xl fade-in">
                    <div class="flex flex-col lg:flex-row lg:justify-between lg:items-start mb-6">
                        <div>
                            <h3 class="font-crimson font-semibold text-2xl mb-2 text-gold-accent">
                                Audit Associate – PIE (Non-FS)
                            </h3>
                            <div class="text-xl text-blue-accent mb-2 premium-text">Grant Thornton Bharat LLP</div>
                        </div>
                        <div class="text-text-secondary font-medium">July 2024 - February 2025</div>
                    </div>
                    <p class="body-text mb-6">
                        Executed comprehensive due diligence and financial analysis for Cipla Group (₹24,000+ crore revenue, NIFTY 50) 
                        and pre-IPO manufacturing company (₹500+ crore revenue). Led inventory verification across multiple locations, 
                        achieving 35% reduction in reporting discrepancies and 100% QA compliance. Developed expertise in valuation 
                        methodologies and working capital optimization essential for investment banking transition.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">Due Diligence</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">Financial Analysis</span>
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">Valuation</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">IPO Preparation</span>
                    </div>
                </div>

                <div class="card-shadow p-8 rounded-xl fade-in">
                    <div class="flex flex-col lg:flex-row lg:justify-between lg:items-start mb-6">
                        <div>
                            <h3 class="font-crimson font-semibold text-2xl mb-2 text-gold-accent">
                                Leadership & Volunteering
                            </h3>
                            <div class="text-xl text-blue-accent mb-2 premium-text">Mulund College Of Commerce</div>
                        </div>
                        <div class="text-text-secondary font-medium">2021 - 2024</div>
                    </div>
                    <p class="body-text mb-6">
                        Active member across multiple departments including Public Relations, Music (SPECTRUM), and Event Management. 
                        Demonstrated leadership in managing PR efforts, contributing to cultural activities, and coordinating college events. 
                        Achieved recognition in beatboxing competitions including Runner Up at SIESONS fest and Third Position at Drop the Beat event.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">Public Relations</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">Event Management</span>
                        <span class="bg-gold-accent bg-opacity-20 text-gold-accent px-4 py-2 rounded-full text-sm font-medium">Cultural Activities</span>
                        <span class="bg-blue-accent bg-opacity-20 text-blue-accent px-4 py-2 rounded-full text-sm font-medium">Leadership</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Certifications Section -->
    <section id="certifications" class="py-20 section-gradient">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="font-crimson font-bold text-5xl mb-4 text-text-primary fade-in">
                    Professional Certifications
                </h2>
                <div class="section-divider w-24 mx-auto mb-8"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="card-shadow p-8 rounded-xl text-center fade-in accent-glow">
                    <div class="text-5xl mb-4">🏆</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">Advanced Diploma in Accounting</h3>
                    <p class="text-blue-accent font-medium mb-2">ACCA (RQF Level 6)</p>
                    <p class="text-text-muted text-sm mb-4">April 2024</p>
                    <p class="body-text text-sm">Advanced qualification demonstrating mastery in financial reporting, audit, and business analysis.</p>
                </div>

                <div class="card-shadow p-8 rounded-xl text-center fade-in">
                    <div class="text-5xl mb-4">📊</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">Goldman Sachs Risk Simulation</h3>
                    <p class="text-blue-accent font-medium mb-2">Forage Platform</p>
                    <p class="text-text-muted text-sm mb-4">April 2025</p>
                    <p class="body-text text-sm">Specialized certification in risk assessment and management within investment banking context.</p>
                </div>

                <div class="card-shadow p-8 rounded-xl text-center fade-in">
                    <div class="text-5xl mb-4">📜</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">Diploma in Accounting</h3>
                    <p class="text-blue-accent font-medium mb-2">ACCA (RQF Level 4)</p>
                    <p class="text-text-muted text-sm mb-4">August 2023</p>
                    <p class="body-text text-sm">Foundation certification in accounting principles and business fundamentals.</p>
                </div>

                <div class="card-shadow p-8 rounded-xl text-center fade-in">
                    <div class="text-5xl mb-4">⚖️</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">Ethics & Professional Skills</h3>
                    <p class="text-blue-accent font-medium mb-2">ACCA (EPSM)</p>
                    <p class="text-text-muted text-sm mb-4">December 2023</p>
                    <p class="body-text text-sm">Professional ethics and skills development for accounting professionals.</p>
                </div>

                <div class="card-shadow p-8 rounded-xl text-center fade-in">
                    <div class="text-5xl mb-4">🎯</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">Foundations in Professionalism</h3>
                    <p class="text-blue-accent font-medium mb-2">ACCA (FIP)</p>
                    <p class="text-text-muted text-sm mb-4">August 2023</p>
                    <p class="body-text text-sm">Core professional development and ethical foundation module.</p>
                </div>

                <div class="card-shadow p-8 rounded-xl text-center fade-in">
                    <div class="text-5xl mb-4">📈</div>
                    <h3 class="font-crimson font-semibold text-xl mb-3 text-gold-accent">ACCA Professional Level</h3>
                    <p class="text-blue-accent font-medium mb-2">11/13 Papers Cleared</p>
                    <p class="text-text-muted text-sm mb-4">2021 - Present</p>
                    <p class="body-text text-sm">Advanced progress through chartered accountancy qualification with focus on corporate finance.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="py-20 bg-dark-primary">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="font-crimson font-bold text-5xl mb-4 text-text-primary fade-in">
                    Core Expertise
                </h2>
                <div class="section-divider w-24 mx-auto mb-8"></div>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="slide-in-left">
                    <h3 class="font-crimson font-semibold text-3xl mb-8 text-gold-accent">
                        Technical Proficiencies
                    </h3>
                    <div class="space-y-8">
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="font-semibold text-text-primary">Risk Assessment</span>
                                <span class="text-gold-accent">95%</span>
                            </div>
                            <div class="bg-dark-accent rounded-full h-3">
                                <div class="progress-bar h-3 rounded-full" data-width="95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="font-semibold text-text-primary">Financial Variance Analysis</span>
                                <span class="text-gold-accent">92%</span>
                            </div>
                            <div class="bg-dark-accent rounded-full h-3">
                                <div class="progress-bar h-3 rounded-full" data-width="92%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="font-semibold text-text-primary">Statutory Audits</span>
                                <span class="text-gold-accent">90%</span>
                            </div>
                            <div class="bg-dark-accent rounded-full h-3">
                                <div class="progress-bar h-3 rounded-full" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="font-semibold text-text-primary">Microsoft Excel & PowerPoint</span>
                                <span class="text-gold-accent">88%</span>
                            </div>
                            <div class="bg-dark-accent rounded-full h-3">
                                <div class="progress-bar h-3 rounded-full" data-width="88%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="font-semibold text-text-primary">Financial Modeling & Valuation</span>
                                <span class="text-gold-accent">85%</span>
                            </div>
                            <div class="bg-dark-accent rounded-full h-3">
                                <div class="progress-bar h-3 rounded-full" data-width="85%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="slide-in-right">
                    <h3 class="font-crimson font-semibold text-3xl mb-8 text-gold-accent">
                        Industry Specialization
                    </h3>
                    <div class="grid grid-cols-2 gap-6">
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">💊</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Pharmaceuticals</h4>
                            <p class="text-sm text-text-secondary">NIFTY 50, Large Cap</p>
                        </div>
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">🏭</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Manufacturing</h4>
                            <p class="text-sm text-text-secondary">Pre-IPO, Mid-Cap</p>
                        </div>
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">📊</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Investment Banking</h4>
                            <p class="text-sm text-text-secondary">M&A, Capital Markets</p>
                        </div>
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">🔍</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Risk Management</h4>
                            <p class="text-sm text-text-secondary">Goldman Sachs Certified</p>
                        </div>
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">🎵</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Leadership</h4>
                            <p class="text-sm text-text-secondary">Cultural & Event Management</p>
                        </div>
                        <div class="card-shadow p-6 rounded-xl text-center">
                            <div class="text-4xl mb-4">⚽</div>
                            <h4 class="font-semibold text-gold-accent mb-2">Team Sports</h4>
                            <p class="text-sm text-text-secondary">Football, Running</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 section-gradient">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="font-crimson font-bold text-5xl mb-4 text-text-primary fade-in">
                    Let's Connect
                </h2>
                <div class="section-divider w-24 mx-auto mb-8"></div>
                <p class="body-text">Ready to discuss investment banking opportunities and strategic partnerships</p>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="slide-in-left">
                    <h3 class="font-crimson font-semibold text-3xl mb-8 text-gold-accent">Get In Touch</h3>
                    <div class="space-y-6">
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-gold-accent rounded-lg flex items-center justify-center mr-4">
                                <span class="text-xl text-dark-primary">📧</span>
                            </div>
                            <div>
                                <div class="font-semibold text-text-primary">Email</div>
                                <div class="text-text-secondary">avandodhia.acca@gmail.com</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-blue-accent rounded-lg flex items-center justify-center mr-4">
                                <span class="text-xl text-white">📱</span>
                            </div>
                            <div>
                                <div class="font-semibold text-text-primary">Phone</div>
                                <div class="text-text-secondary">+91 9004628904</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-gold-accent rounded-lg flex items-center justify-center mr-4">
                                <span class="text-xl text-dark-primary">📍</span>
                            </div>
                            <div>
                                <div class="font-semibold text-text-primary">Location</div>
                                <div class="text-text-secondary">Mumbai, India</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-blue-accent rounded-lg flex items-center justify-center mr-4">
                                <span class="text-xl text-white">💼</span>
                            </div>
                            <div>
                                <div class="font-semibold text-text-primary">LinkedIn</div>
                                <div class="text-text-secondary">linkedin.com/in/avan-dodhia</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="slide-in-right">
                    <form class="space-y-6" id="contact-form">
                        <div>
                            <input type="text" placeholder="Your Name" 
                                   class="w-full px-4 py-3 bg-dark-accent border border-text-muted rounded-lg focus:border-gold-accent focus:outline-none transition-colors text-text-primary placeholder-text-muted" required>
                        </div>
                        <div>
                            <input type="email" placeholder="Your Email" 
                                   class="w-full px-4 py-3 bg-dark-accent border border-text-muted rounded-lg focus:border-gold-accent focus:outline-none transition-colors text-text-primary placeholder-text-muted" required>
                        </div>
                        <div>
                            <input type="text" placeholder="Company" 
                                   class="w-full px-4 py-3 bg-dark-accent border border-text-muted rounded-lg focus:border-gold-accent focus:outline-none transition-colors text-text-primary placeholder-text-muted">
                        </div>
                        <div>
                            <textarea rows="4" placeholder="Your Message" 
                                      class="w-full px-4 py-3 bg-dark-accent border border-text-muted rounded-lg focus:border-gold-accent focus:outline-none transition-colors resize-none text-text-primary placeholder-text-muted" required></textarea>
                        </div>
                        <button type="submit" class="w-full btn-primary py-3 rounded-lg font-semibold text-lg">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark-primary py-12 border-t border-dark-accent">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-3 gap-8 mb-8">
                <div>
                    <h3 class="font-crimson font-bold text-xl text-gold-accent mb-4">Avan Dodhia</h3>
                    <p class="text-text-secondary text-sm leading-relaxed">
                        Investment Banking Fellow specializing in M&A advisory, financial modeling, and capital markets. 
                        ACCA Professional with Goldman Sachs certification.
                    </p>
                </div>
                <div>
                    <h4 class="font-semibold text-text-primary mb-4">Quick Links</h4>
                    <div class="space-y-2">
                        <a href="#about" class="block text-text-secondary hover:text-gold-accent transition-colors text-sm">About</a>
                        <a href="#experience" class="block text-text-secondary hover:text-gold-accent transition-colors text-sm">Experience</a>
                        <a href="#certifications" class="block text-text-secondary hover:text-gold-accent transition-colors text-sm">Certifications</a>
                        <a href="#expertise" class="block text-text-secondary hover:text-gold-accent transition-colors text-sm">Expertise</a>
                    </div>
                </div>
                <div>
                    <h4 class="font-semibold text-text-primary mb-4">Connect</h4>
                    <div class="space-y-2">
                        <p class="text-text-secondary text-sm">avandodhia.acca@gmail.com</p>
                        <p class="text-text-secondary text-sm">+91 9004628904</p>
                        <p class="text-text-secondary text-sm">Mumbai, India</p>
                    </div>
                </div>
            </div>
            <div class="border-t border-dark-accent pt-8 text-center">
                <p class="text-text-muted text-sm">&copy; 2024 Avan Dodhia. All rights reserved. • Investment Banking Professional • ACCA Qualified</p>
            </div>
        </div>
    </footer>

    <script>
        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observe all animated elements
        document.querySelectorAll('.fade-in, .slide-in-left, .slide-in-right').forEach(el => {
            observer.observe(el);
        });

        // Progress bars animation
        const progressObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const progressBars = entry.target.querySelectorAll('.progress-bar');
                    progressBars.forEach(bar => {
                        const width = bar.getAttribute('data-width');
                        setTimeout(() => {
                            bar.style.width = width;
                        }, 500);
                    });
                }
            });
        }, { threshold: 0.5 });

        document.querySelector('#expertise').addEventListener('scroll', () => {
            progressObserver.observe(document.querySelector('#expertise'));
        });

        // Trigger progress bars when section is visible
        observer.observe(document.querySelector('#expertise'));
        
        // Mobile menu toggle
        document.getElementById('mobile-menu').addEventListener('click', function() {
            // Add mobile menu functionality here
            console.log('Mobile menu clicked');
        });

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Contact form handling
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! I will get back to you soon.');
            this.reset();
        });

        // Trigger progress bars when expertise section comes into view
        const expertiseSection = document.querySelector('#expertise');
        const progressBarsTriggered = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const progressBars = document.querySelectorAll('.progress-bar');
                    progressBars.forEach(bar => {
                        const width = bar.getAttribute('data-width');
                        setTimeout(() => {
                            bar.style.width = width;
                        }, 800);
                    });
                }
            });
        }, { threshold: 0.3 });

        progressBarsTriggered.observe(expertiseSection);
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'96c5ccba978c3501',t:'MTc1NDcyNzI2NC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
