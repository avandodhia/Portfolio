<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avan Dodhia - Investment Banking Analyst</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .section-divider {
            width: 60px;
            height: 2px;
            background: linear-gradient(90deg, #1e3a8a, #d4af37);
            margin: 2rem auto;
        }
        
        .nav-blur {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        }
        
        .card-hover {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }
        
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -8px;
            top: 0;
            width: 16px;
            height: 16px;
            background: linear-gradient(135deg, #1e3a8a, #d4af37);
            border-radius: 50%;
            border: 3px solid white;
            box-shadow: 0 0 0 3px rgba(30, 58, 138, 0.2);
        }
        
        .timeline-line {
            position: absolute;
            left: 0;
            top: 20px;
            bottom: -20px;
            width: 2px;
            background: linear-gradient(to bottom, #1e3a8a, #d4af37);
        }
        
        .cert-card {
            background: linear-gradient(145deg, #ffffff, #f8fafc);
            border: 1px solid rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .cert-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.1);
            border-color: #d4af37;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #334155 100%);
        }
        
        .text-gradient {
            background: linear-gradient(135deg, #1e3a8a, #d4af37);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .project-card {
            background: white;
            border: 1px solid rgba(0, 0, 0, 0.08);
            transition: all 0.4s ease;
        }
        
        .project-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 16px 32px rgba(0, 0, 0, 0.12);
            border-color: rgba(212, 175, 55, 0.3);
        }
        
        .contact-item {
            transition: all 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateX(8px);
            color: #1e3a8a;
        }
        
        /* Desktop optimizations - Fixed for proper scaling */
        @media (min-width: 1024px) {
            .hero-text {
                font-size: 4rem;
                line-height: 1.1;
            }
            
            .section-padding {
                padding: 5rem 2rem;
            }
            
            .max-w-6xl {
                max-width: 1200px;
            }
            
            .max-w-4xl {
                max-width: 900px;
            }
        }
        
        @media (min-width: 1280px) {
            .hero-text {
                font-size: 5rem;
            }
            
            .section-padding {
                padding: 6rem 2rem;
            }
            
            .max-w-6xl {
                max-width: 1400px;
            }
            
            .max-w-4xl {
                max-width: 1100px;
            }
        }
        
        @media (max-width: 768px) {
            .hero-text {
                font-size: 2.5rem;
            }
            
            .section-padding {
                padding: 4rem 1rem;
            }
        }
        
        .smooth-appear {
            animation: smoothAppear 1s ease-out forwards;
        }
        
        @keyframes smoothAppear {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .stagger-1 { animation-delay: 0.1s; }
        .stagger-2 { animation-delay: 0.2s; }
        .stagger-3 { animation-delay: 0.3s; }
        .stagger-4 { animation-delay: 0.4s; }
        
        .icon-finance {
            background: linear-gradient(135deg, #1e3a8a, #3b82f6);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .photo-zoom {
            animation: photoZoomIn 1.2s ease-out forwards;
            transform: scale(0.8);
            opacity: 0;
        }
        
        @keyframes photoZoomIn {
            0% {
                transform: scale(0.8);
                opacity: 0;
            }
            60% {
                transform: scale(1.05);
                opacity: 0.8;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }
        
        .photo-glow {
            box-shadow: 0 0 40px rgba(212, 175, 55, 0.3), 0 0 80px rgba(30, 58, 138, 0.2);
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full nav-blur z-50 transition-all duration-300">
        <div class="container nav-desktop">
            <div class="flex justify-between items-center">
                <a href="#home" class="text-2xl font-bold text-gray-900 hover:text-blue-900 transition-colors">
                    Avan Dodhia
                </a>
                <div class="hidden lg:flex space-x-10">
                    <a href="#about" class="text-gray-700 hover:text-blue-900 transition-colors font-medium text-lg">About</a>
                    <a href="#projects" class="text-gray-700 hover:text-blue-900 transition-colors font-medium text-lg">Projects</a>
                    <a href="#experience" class="text-gray-700 hover:text-blue-900 transition-colors font-medium text-lg">Experience</a>
                    <a href="#certifications" class="text-gray-700 hover:text-blue-900 transition-colors font-medium text-lg">Certifications</a>
                    <a href="#contact" class="text-gray-700 hover:text-blue-900 transition-colors font-medium text-lg">Contact</a>
                </div>
                <button class="lg:hidden text-gray-700 p-2" onclick="toggleMobileMenu()">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
            <!-- Mobile Menu -->
            <div class="mobile-menu" id="mobileMenu">
                <a href="#about" onclick="closeMobileMenu()">About</a>
                <a href="#projects" onclick="closeMobileMenu()">Projects</a>
                <a href="#experience" onclick="closeMobileMenu()">Experience</a>
                <a href="#certifications" onclick="closeMobileMenu()">Certifications</a>
                <a href="#contact" onclick="closeMobileMenu()">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient flex items-center justify-center text-white">
        <div class="container-xl px-6 py-20">
            <div class="desktop-grid items-center min-h-screen">
                <!-- Left Column - Professional Photo -->
                <div class="flex justify-center lg:justify-end fade-in smooth-appear order-2 lg:order-1">
                    <div class="relative">
                        <div class="w-80 h-80 lg:w-96 lg:h-96 xl:w-[28rem] xl:h-[28rem] rounded-full overflow-hidden border-4 border-white/20 shadow-2xl photo-glow relative">
                            <div class="absolute inset-0 bg-gradient-to-br from-blue-600/20 to-yellow-500/20 rounded-full"></div>
                            <img src="your-profile-photo.jpg" 
                                 alt="Avan Dodhia - Professional Headshot" 
                                 class="w-full h-full object-cover rounded-full relative z-10 photo-zoom"
                                 onerror="this.src=''; this.alt='Upload your photo here'; this.style.background='linear-gradient(135deg, #1e3a8a, #d4af37)'; this.style.display='flex'; this.style.alignItems='center'; this.style.justifyContent='center'; this.style.fontSize='5rem'; this.innerHTML='📸'; this.style.color='white';">
                        </div>
                        <!-- Enhanced Decorative elements -->
                        <div class="absolute -top-6 -right-6 w-12 h-12 bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-full opacity-80 animate-pulse"></div>
                        <div class="absolute -bottom-8 -left-8 w-16 h-16 bg-gradient-to-br from-blue-400 to-blue-600 rounded-full opacity-60 animate-pulse" style="animation-delay: 0.5s;"></div>
                        <div class="absolute top-1/2 -left-10 w-8 h-8 bg-gradient-to-br from-white to-gray-200 rounded-full opacity-40 animate-pulse" style="animation-delay: 1s;"></div>
                    </div>
                </div>
                
                <!-- Right Column - Introduction Text -->
                <div class="text-center lg:text-left fade-in smooth-appear stagger-1 order-1 lg:order-2">
                    <h1 class="hero-text text-5xl lg:text-6xl xl:text-7xl font-black mb-8 leading-tight">
                        Avan Dodhia
                    </h1>
                    <p class="text-xl lg:text-2xl xl:text-3xl mb-10 text-blue-100 font-light leading-relaxed">
                        Aspiring Investment Banking Analyst | ACCA Candidate | Audit Associate
                    </p>
                    <div class="mb-12 stagger-2 smooth-appear space-y-6">
                        <p class="text-lg lg:text-xl leading-relaxed text-gray-300">
                            Finance professional with experience auditing Fortune 500 companies at Grant Thornton. 
                            Passionate about transitioning into investment banking, with expertise in financial analysis, 
                            IFRS compliance, and M&A valuations.
                        </p>
                        <p class="text-lg lg:text-xl leading-relaxed text-gray-300">
                            Currently pursuing ACCA professional qualification with 11 of 13 papers cleared, 
                            combining strong analytical skills with hands-on experience in corporate finance 
                            and regulatory compliance.
                        </p>
                    </div>
                    <div class="flex flex-col sm:flex-row gap-6 justify-center lg:justify-start stagger-3 smooth-appear">
                        <a href="#projects" class="btn-primary text-lg">
                            View My Work
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
                            </svg>
                        </a>
                        <a href="#contact" class="btn-secondary text-lg">
                            Get In Touch
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section-padding bg-gray-50">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">About</h2>
                <div class="section-divider"></div>
            </div>
            
            <div class="desktop-grid">
                <div class="fade-in">
                    <div class="w-full h-96 bg-gradient-to-br from-blue-900 to-blue-700 rounded-3xl flex items-center justify-center text-white shadow-2xl">
                        <div class="text-center">
                            <div class="text-8xl mb-6 icon-finance">📊</div>
                            <div class="text-2xl font-semibold">Finance Professional</div>
                        </div>
                    </div>
                </div>
                
                <div class="fade-in">
                    <h3 class="text-3xl lg:text-4xl font-bold text-gray-900 mb-8">Finance Professional & ACCA Candidate</h3>
                    <p class="text-gray-600 mb-8 leading-relaxed text-lg">
                        B.Com graduate with specialized expertise in financial audits, IFRS compliance, and variance analysis. 
                        Currently working as an Audit Associate at Grant Thornton Bharat LLP, where I've audited major 
                        corporations including Cipla (₹24,000 Cr revenue) and IPO-preparing firms.
                    </p>
                    <p class="text-gray-600 mb-10 leading-relaxed text-lg">
                        My passion lies in investment banking, particularly M&A transactions and valuations. 
                        I'm actively pursuing my ACCA professional qualification and have completed virtual 
                        internships with Goldman Sachs to deepen my understanding of risk management and capital markets.
                    </p>
                    
                    <div class="grid grid-cols-2 gap-6">
                        <div class="text-center p-6 bg-white rounded-2xl shadow-lg">
                            <div class="text-3xl font-bold text-blue-900 mb-2">11/13</div>
                            <div class="text-gray-600 font-medium">ACCA Papers</div>
                        </div>
                        <div class="text-center p-6 bg-white rounded-2xl shadow-lg">
                            <div class="text-3xl font-bold text-blue-900 mb-2">₹24K+ Cr</div>
                            <div class="text-gray-600 font-medium">Assets Audited</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="section-padding bg-white">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">Projects</h2>
                <div class="section-divider"></div>
                <p class="text-xl lg:text-2xl text-gray-600 max-w-3xl mx-auto">
                    Key financial projects demonstrating expertise in audit, compliance, and analysis
                </p>
            </div>
            
            <div class="project-grid">
                <div class="project-card rounded-3xl p-8 fade-in card-hover">
                    <div class="text-5xl mb-8 text-center">🏭</div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">Large-Cap Pharmaceutical Audit</h3>
                    <div class="mb-6">
                        <span class="inline-block px-4 py-2 bg-blue-100 text-blue-800 rounded-full text-sm font-semibold">
                            ₹24,000+ Cr Revenue
                        </span>
                    </div>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        Led comprehensive statutory audit for Cipla, including multi-location inventory verification, 
                        IFRS compliance review, and stakeholder reporting across 4 major depots.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-blue-500 rounded-full mr-3"></span>
                            Financial statement analysis
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-blue-500 rounded-full mr-3"></span>
                            Inventory verification
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-blue-500 rounded-full mr-3"></span>
                            Compliance assessment
                        </li>
                    </ul>
                </div>
                
                <div class="project-card rounded-3xl p-8 fade-in card-hover">
                    <div class="text-5xl mb-8 text-center">🚀</div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">IPO Preparation Advisory</h3>
                    <div class="mb-6">
                        <span class="inline-block px-4 py-2 bg-green-100 text-green-800 rounded-full text-sm font-semibold">
                            ₹500+ Cr Revenue
                        </span>
                    </div>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        Supported IPO-preparing manufacturing firm through comprehensive audit processes, 
                        compliance framework enhancement, and financial reporting optimization.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-green-500 rounded-full mr-3"></span>
                            IPO readiness assessment
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-green-500 rounded-full mr-3"></span>
                            Due diligence support
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-green-500 rounded-full mr-3"></span>
                            Regulatory compliance
                        </li>
                    </ul>
                </div>
                
                <div class="project-card rounded-3xl p-8 fade-in card-hover">
                    <div class="text-5xl mb-8 text-center">📈</div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">Process Optimization</h3>
                    <div class="mb-6">
                        <span class="inline-block px-4 py-2 bg-yellow-100 text-yellow-800 rounded-full text-sm font-semibold">
                            35% Efficiency Gain
                        </span>
                    </div>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        Identified and implemented process improvements across audit workflows, 
                        resulting in significant efficiency gains and enhanced quality assurance.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-yellow-500 rounded-full mr-3"></span>
                            Workflow optimization
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-yellow-500 rounded-full mr-3"></span>
                            KPI benchmarking
                        </li>
                        <li class="flex items-center">
                            <span class="w-2 h-2 bg-yellow-500 rounded-full mr-3"></span>
                            Quality enhancement
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Highlights Section -->
    <section class="section-padding bg-gray-50">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">Highlights</h2>
                <div class="section-divider"></div>
            </div>
            
            <div class="desktop-3-col gap-8">
                <div class="text-center fade-in">
                    <div class="w-24 h-24 bg-gradient-to-br from-blue-900 to-blue-700 rounded-3xl flex items-center justify-center text-white text-4xl mx-auto mb-6 shadow-xl">
                        🏆
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">ACCA Excellence</h3>
                    <p class="text-gray-600">11 of 13 professional papers cleared with distinction</p>
                </div>
                
                <div class="text-center fade-in">
                    <div class="w-24 h-24 bg-gradient-to-br from-yellow-600 to-yellow-500 rounded-3xl flex items-center justify-center text-white text-4xl mx-auto mb-6 shadow-xl">
                        💼
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Professional Experience</h3>
                    <p class="text-gray-600">Grant Thornton Audit Associate with Fortune 500 exposure</p>
                </div>
                
                <div class="text-center fade-in">
                    <div class="w-24 h-24 bg-gradient-to-br from-green-600 to-green-500 rounded-3xl flex items-center justify-center text-white text-4xl mx-auto mb-6 shadow-xl">
                        📊
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Impact Delivered</h3>
                    <p class="text-gray-600">35% efficiency improvement in audit processes</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="section-padding bg-white">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">Experience</h2>
                <div class="section-divider"></div>
            </div>
            
            <div class="max-w-4xl mx-auto">
                <div class="relative pl-12">
                    <div class="timeline-line"></div>
                    
                    <div class="relative timeline-item fade-in">
                        <div class="bg-white rounded-3xl p-10 shadow-xl border-2 border-gray-100 mb-8">
                            <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between mb-8">
                                <div>
                                    <h3 class="text-3xl font-bold text-gray-900 mb-3">Audit Associate</h3>
                                    <h4 class="text-xl text-gray-600 font-semibold">Grant Thornton Bharat LLP</h4>
                                </div>
                                <div class="mt-6 lg:mt-0">
                                    <span class="inline-block px-6 py-3 bg-blue-100 text-blue-800 rounded-full font-semibold">
                                        July 2024 – Feb 2025
                                    </span>
                                </div>
                            </div>
                            
                            <div class="space-y-6">
                                <div class="flex items-start">
                                    <span class="text-green-500 mr-4 mt-1 text-xl">✓</span>
                                    <span class="text-gray-700 text-lg">Audited large-scale clients including Cipla (₹24,000 Cr revenue) and IPO-preparing firms</span>
                                </div>
                                <div class="flex items-start">
                                    <span class="text-green-500 mr-4 mt-1 text-xl">✓</span>
                                    <span class="text-gray-700 text-lg">Reduced reporting discrepancies by 35% through comprehensive inventory verification</span>
                                </div>
                                <div class="flex items-start">
                                    <span class="text-green-500 mr-4 mt-1 text-xl">✓</span>
                                    <span class="text-gray-700 text-lg">Delivered variance analysis across 5+ OpEx categories for 12+ stakeholders</span>
                                </div>
                                <div class="flex items-start">
                                    <span class="text-green-500 mr-4 mt-1 text-xl">✓</span>
                                    <span class="text-gray-700 text-lg">Enhanced compliance frameworks resulting in 20% boost in audit readiness</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Certifications Section -->
    <section id="certifications" class="section-padding bg-gray-50">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">Certifications</h2>
                <div class="section-divider"></div>
                <p class="text-xl lg:text-2xl text-gray-600">Professional qualifications and continuous learning</p>
            </div>
            
            <div class="desktop-3-col gap-8">
                <div class="cert-card rounded-3xl p-10 fade-in" onclick="openCertificate('acca')">
                    <div class="text-center">
                        <div class="w-20 h-20 bg-gradient-to-br from-blue-900 to-blue-700 rounded-3xl flex items-center justify-center text-white text-3xl mx-auto mb-8">
                            🎓
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-4">ACCA Professional</h3>
                        <p class="text-gray-600 mb-6 text-lg">Advanced Diploma in Accounting and Business</p>
                        <div class="text-blue-600 font-semibold text-lg">11/13 Papers Cleared</div>
                        <div class="mt-6 text-sm text-gray-500">Click to view certificate</div>
                    </div>
                </div>
                
                <div class="cert-card rounded-3xl p-10 fade-in" onclick="openCertificate('epsm')">
                    <div class="text-center">
                        <div class="w-20 h-20 bg-gradient-to-br from-green-600 to-green-500 rounded-3xl flex items-center justify-center text-white text-3xl mx-auto mb-8">
                            📊
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-4">EPSM Certification</h3>
                        <p class="text-gray-600 mb-6 text-lg">Enterprise Performance & Strategy Management</p>
                        <div class="text-green-600 font-semibold text-lg">Completed</div>
                        <div class="mt-6 text-sm text-gray-500">Click to view certificate</div>
                    </div>
                </div>
                
                <div class="cert-card rounded-3xl p-10 fade-in" onclick="openCertificate('goldman')">
                    <div class="text-center">
                        <div class="w-20 h-20 bg-gradient-to-br from-yellow-600 to-yellow-500 rounded-3xl flex items-center justify-center text-white text-3xl mx-auto mb-8">
                            🏛️
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-4">Goldman Sachs</h3>
                        <p class="text-gray-600 mb-6 text-lg">Risk Management Virtual Internship</p>
                        <div class="text-yellow-600 font-semibold text-lg">Forage Platform</div>
                        <div class="mt-6 text-sm text-gray-500">Click to view certificate</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section-padding bg-white">
        <div class="container">
            <div class="text-center mb-20 fade-in">
                <h2 class="text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900 mb-6">Contact</h2>
                <div class="section-divider"></div>
                <p class="text-xl lg:text-2xl text-gray-600">Let's discuss opportunities in investment banking and finance</p>
            </div>
            
            <div class="desktop-grid gap-16">
                <div class="space-y-8 fade-in">
                    <div class="contact-item flex items-center space-x-6">
                        <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center text-blue-600 text-2xl">
                            📧
                        </div>
                        <div>
                            <p class="font-bold text-gray-900 text-lg">Email</p>
                            <a href="mailto:avandodhia.acca@gmail.com" class="text-gray-600 hover:text-blue-600 transition-colors text-lg">
                                avandodhia.acca@gmail.com
                            </a>
                        </div>
                    </div>
                    
                    <div class="contact-item flex items-center space-x-6">
                        <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center text-blue-600 text-2xl">
                            💼
                        </div>
                        <div>
                            <p class="font-bold text-gray-900 text-lg">LinkedIn</p>
                            <a href="https://linkedin.com/in/avan-dodhia" target="_blank" class="text-gray-600 hover:text-blue-600 transition-colors text-lg">
                                linkedin.com/in/avan-dodhia
                            </a>
                        </div>
                    </div>
                    
                    <div class="contact-item flex items-center space-x-6">
                        <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center text-blue-600 text-2xl">
                            📱
                        </div>
                        <div>
                            <p class="font-bold text-gray-900 text-lg">Phone</p>
                            <a href="tel:+919004628904" class="text-gray-600 hover:text-blue-600 transition-colors text-lg">
                                +91 9004628904
                            </a>
                        </div>
                    </div>
                    
                    <div class="contact-item flex items-center space-x-6">
                        <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center text-blue-600 text-2xl">
                            📍
                        </div>
                        <div>
                            <p class="font-bold text-gray-900 text-lg">Location</p>
                            <p class="text-gray-600 text-lg">Mumbai, India</p>
                        </div>
                    </div>
                </div>
                
                <div class="fade-in">
                    <div class="bg-gray-50 rounded-3xl p-10">
                        <h3 class="text-3xl font-bold text-gray-900 mb-8">Let's Connect</h3>
                        <p class="text-gray-600 mb-10 leading-relaxed text-lg">
                            I'm actively seeking opportunities in investment banking, particularly in M&A, 
                            valuations, and capital markets. Let's discuss how my audit experience and 
                            financial expertise can contribute to your team.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-6">
                            <a href="mailto:avandodhia.acca@gmail.com" class="btn-primary text-lg">
                                Send Email
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
                                </svg>
                            </a>
                            <a href="https://linkedin.com/in/avan-dodhia" target="_blank" class="btn-secondary text-lg" style="color: #1e3a8a; border-color: #1e3a8a;">
                                LinkedIn Profile
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-16">
        <div class="container text-center">
            <div class="mb-10">
                <h3 class="text-3xl font-bold mb-4">Avan Dodhia</h3>
                <p class="text-gray-400 text-lg">Aspiring Investment Banking Analyst | ACCA Candidate | Audit Associate</p>
            </div>
            <div class="border-t border-gray-800 pt-10">
                <p class="text-gray-500">© 2024 Avan Dodhia. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu functions
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('active');
        }

        function closeMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.remove('active');
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    const navHeight = document.querySelector('nav').offsetHeight;
                    const targetPosition = target.offsetTop - navHeight;
                    window.scrollTo({
                        top: targetPosition,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Enhanced fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Enhanced navigation background on scroll
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.style.background = 'rgba(255, 255, 255, 0.98)';
                nav.style.boxShadow = '0 4px 20px rgba(0, 0, 0, 0.1)';
            } else {
                nav.style.background = 'rgba(255, 255, 255, 0.95)';
                nav.style.boxShadow = '0 2px 20px rgba(0, 0, 0, 0.05)';
            }
        });

        // Certificate click handlers with enhanced messages
        function openCertificate(type) {
            let message = '';
            switch(type) {
                case 'acca':
                    message = 'ACCA Professional Qualification\n\n✓ 11 of 13 papers cleared with distinction\n✓ Specializing in Financial Reporting, Audit & Assurance, and Strategic Business Management\n✓ Advanced knowledge in IFRS, corporate governance, and risk management\n✓ Expected completion: 2025';
                    break;
                case 'epsm':
                    message = 'Enterprise Performance & Strategy Management Certification\n\n✓ Advanced training in business strategy and performance measurement\n✓ Management consulting methodologies\n✓ Strategic planning and execution frameworks\n✓ KPI development and benchmarking';
                    break;
                case 'goldman':
                    message = 'Goldman Sachs Risk Management Virtual Internship\n\n✓ Comprehensive training in financial risk assessment\n✓ Portfolio management and optimization\n✓ Investment banking practices and methodologies\n✓ Capital markets and trading strategies\n✓ Completed through Forage platform';
                    break;
            }
            alert(message + '\n\n📄 Note: This is a portfolio demonstration. In the live version, this would open the actual certificate document or verification link.');
        }

        // Initialize animations on load
        window.addEventListener('load', () => {
            // Trigger animations for elements already in view
            document.querySelectorAll('.fade-in').forEach(el => {
                const rect = el.getBoundingClientRect();
                if (rect.top < window.innerHeight && rect.bottom > 0) {
                    el.classList.add('visible');
                }
            });
        });

        // Close mobile menu when clicking outside
        document.addEventListener('click', function(event) {
            const nav = document.querySelector('nav');
            const menu = document.getElementById('mobileMenu');
            const button = document.querySelector('nav button');
            
            if (!nav.contains(event.target) && menu.classList.contains('active')) {
                menu.classList.remove('active');
            }
        });

        // Enhanced scroll performance
        let ticking = false;
        function updateOnScroll() {
            // Navigation background update
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.style.background = 'rgba(255, 255, 255, 0.98)';
                nav.style.boxShadow = '0 4px 20px rgba(0, 0, 0, 0.1)';
            } else {
                nav.style.background = 'rgba(255, 255, 255, 0.95)';
                nav.style.boxShadow = '0 2px 20px rgba(0, 0, 0, 0.05)';
            }
            ticking = false;
        }

        window.addEventListener('scroll', () => {
            if (!ticking) {
                requestAnimationFrame(updateOnScroll);
                ticking = true;
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9761ff87c7312e8f',t:'MTc1NjM2NTEyNC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
