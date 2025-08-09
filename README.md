<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avan Dodhia - Finance Professional</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700;900&family=Crimson+Text:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body { 
            font-family: 'Crimson Text', serif; 
            background: #000;
            color: #fff;
        }
        .prestige-font { font-family: 'Playfair Display', serif; }
        
        /* Elegant animations */
        .slide-up {
            opacity: 0;
            transform: translateY(60px);
            transition: all 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .slide-up.animate {
            opacity: 1;
            transform: translateY(0);
        }
        
        .fade-in-left {
            opacity: 0;
            transform: translateX(-50px);
            transition: all 1s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .fade-in-left.animate {
            opacity: 1;
            transform: translateX(0);
        }
        
        .fade-in-right {
            opacity: 0;
            transform: translateX(50px);
            transition: all 1s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .fade-in-right.animate {
            opacity: 1;
            transform: translateX(0);
        }
        
        .scale-in {
            opacity: 0;
            transform: scale(0.8);
            transition: all 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .scale-in.animate {
            opacity: 1;
            transform: scale(1);
        }
        
        /* Luxury hover effects */
        .luxury-hover {
            transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
            position: relative;
            overflow: hidden;
        }
        .luxury-hover::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
            transition: left 0.6s;
        }
        .luxury-hover:hover::before {
            left: 100%;
        }
        .luxury-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(255,255,255,0.1);
        }
        
        /* Elegant borders */
        .elegant-border {
            position: relative;
        }
        .elegant-border::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border: 1px solid rgba(255,255,255,0.2);
            transition: all 0.3s ease;
        }
        .elegant-border:hover::before {
            border-color: rgba(255,255,255,0.6);
        }
        
        /* Typing animation */
        .typewriter {
            overflow: hidden;
            border-right: 2px solid rgba(255,255,255,0.75);
            white-space: nowrap;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: rgba(255,255,255,0.75); }
        }
        
        /* Floating elements */
        .float {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        
        /* Progress bars */
        .progress-bar {
            width: 0%;
            transition: width 2s cubic-bezier(0.25, 0.46, 0.45, 0.94);
            background: linear-gradient(90deg, #fff, rgba(255,255,255,0.7));
        }
        
        /* Staggered animations */
        .stagger-1 { animation-delay: 0.1s; }
        .stagger-2 { animation-delay: 0.2s; }
        .stagger-3 { animation-delay: 0.3s; }
        .stagger-4 { animation-delay: 0.4s; }
        .stagger-5 { animation-delay: 0.5s; }
        
        /* Elegant underlines */
        .elegant-underline {
            position: relative;
        }
        .elegant-underline::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 0;
            height: 2px;
            background: #fff;
            transition: width 0.3s ease;
        }
        .elegant-underline:hover::after {
            width: 100%;
        }
        
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #111;
        }
        ::-webkit-scrollbar-thumb {
            background: #333;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #555;
        }
    </style>
</head>
<body class="bg-black text-white">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-black bg-opacity-95 backdrop-blur-sm z-50 border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <h1 class="text-2xl prestige-font font-bold tracking-wider">AVAN DODHIA</h1>
                <div class="hidden md:flex space-x-8">
                    <a href="#about" class="elegant-underline text-gray-300 hover:text-white transition-colors duration-300">About</a>
                    <a href="#experience" class="elegant-underline text-gray-300 hover:text-white transition-colors duration-300">Experience</a>
                    <a href="#expertise" class="elegant-underline text-gray-300 hover:text-white transition-colors duration-300">Expertise</a>
                    <a href="#achievements" class="elegant-underline text-gray-300 hover:text-white transition-colors duration-300">Achievements</a>
                    <a href="#contact" class="elegant-underline text-gray-300 hover:text-white transition-colors duration-300">Contact</a>
                </div>
                <button id="mobile-menu-btn" class="md:hidden text-white">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
            <div id="mobile-menu" class="hidden md:hidden mt-4 space-y-2 border-t border-gray-800 pt-4">
                <a href="#about" class="block py-2 text-gray-300 hover:text-white">About</a>
                <a href="#experience" class="block py-2 text-gray-300 hover:text-white">Experience</a>
                <a href="#expertise" class="block py-2 text-gray-300 hover:text-white">Expertise</a>
                <a href="#achievements" class="block py-2 text-gray-300 hover:text-white">Achievements</a>
                <a href="#contact" class="block py-2 text-gray-300 hover:text-white">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="min-h-screen flex items-center justify-center relative overflow-hidden">
        <div class="absolute inset-0 bg-gradient-to-br from-gray-900 via-black to-gray-900"></div>
        <div class="relative z-10 text-center max-w-4xl mx-auto px-6">
            <div class="slide-up">
                <h1 class="prestige-font text-6xl md:text-8xl font-bold mb-6 tracking-wider">
                    AVAN DODHIA
                </h1>
                <div class="typewriter prestige-font text-2xl md:text-3xl text-gray-300 mb-8 inline-block">
                    ACCA Trainee & Finance Professional
                </div>
                <p class="text-xl md:text-2xl text-gray-400 mb-12 leading-relaxed max-w-3xl mx-auto">
                    Delivering precision in audit excellence and financial reporting for leading corporations across diverse industries
                </p>
                <div class="space-x-6">
                    <a href="#experience" class="luxury-hover elegant-border inline-block px-8 py-4 text-lg font-semibold tracking-wider transition-all duration-300">
                        VIEW PORTFOLIO
                    </a>
                    <a href="#contact" class="luxury-hover bg-white text-black inline-block px-8 py-4 text-lg font-semibold tracking-wider transition-all duration-300">
                        CONNECT
                    </a>
                </div>
            </div>
        </div>
        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 float">
            <svg class="w-6 h-6 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
            </svg>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-24 bg-gradient-to-b from-black to-gray-900">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="slide-up prestige-font text-5xl font-bold mb-6 tracking-wider">DISTINGUISHED PROFILE</h2>
                <div class="slide-up w-24 h-0.5 bg-white mx-auto"></div>
            </div>
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="fade-in-left">
                    <div class="text-6xl mb-8 text-center">📊</div>
                    <div class="space-y-6 text-lg leading-relaxed">
                        <p class="text-gray-300">
                            As an ACCA Trainee with Grant Thornton Bharat LLP, I bring precision and analytical rigor to audit and financial reporting for major corporations, including NIFTY 50 companies with revenues exceeding ₹24,000 crores.
                        </p>
                        <p class="text-gray-300">
                            My expertise spans statutory audits, internal controls assessment, cost variance analysis, and financial due diligence across pharmaceuticals and manufacturing sectors, with a strong foundation in ACCA professional standards.
                        </p>
                        <p class="text-gray-300">
                            Currently pursuing ACCA qualification (11/13 papers cleared) while gaining hands-on experience in audit execution, stakeholder reporting, and process optimization for leading Indian corporations.
                        </p>
                    </div>
                </div>
                <div class="fade-in-right">
                    <div class="grid grid-cols-2 gap-8">
                        <div class="luxury-hover elegant-border p-6 text-center">
                            <div class="prestige-font text-4xl font-bold mb-2">₹24,500+</div>
                            <div class="text-gray-400 text-sm tracking-wider">CRORES AUDITED</div>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-1">
                            <div class="prestige-font text-4xl font-bold mb-2">11/13</div>
                            <div class="text-gray-400 text-sm tracking-wider">ACCA PAPERS</div>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-2">
                            <div class="prestige-font text-4xl font-bold mb-2">35%</div>
                            <div class="text-gray-400 text-sm tracking-wider">DISCREPANCY REDUCTION</div>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-3">
                            <div class="prestige-font text-4xl font-bold mb-2">100%</div>
                            <div class="text-gray-400 text-sm tracking-wider">QA COMPLIANCE</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-24 bg-black">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="slide-up prestige-font text-5xl font-bold mb-6 tracking-wider">PROFESSIONAL JOURNEY</h2>
                <div class="slide-up w-24 h-0.5 bg-white mx-auto"></div>
            </div>
            <div class="space-y-12">
                <div class="luxury-hover elegant-border p-8 fade-in-left">
                    <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between mb-6">
                        <div>
                            <h3 class="prestige-font text-3xl font-bold mb-2">ACCA Trainee, Audit – PIE (Non-FS)</h3>
                            <p class="text-xl text-gray-300">Grant Thornton Bharat LLP</p>
                        </div>
                        <span class="text-gray-400 text-lg tracking-wider">July 2024 - February 2025</span>
                    </div>
                    <p class="text-gray-300 text-lg leading-relaxed mb-6">
                        Executed statutory audit procedures for Cipla Group (₹24,000+ crore revenue, NIFTY 50) and a private manufacturing company (₹500+ crore revenue) preparing for listing. Led inventory verification across 4 depots/plants, achieving 100% accuracy and reducing discrepancies by 35%.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">STATUTORY AUDIT</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">INVENTORY VERIFICATION</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">COST VARIANCE ANALYSIS</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">INTERNAL CONTROLS</span>
                    </div>
                </div>

                <div class="luxury-hover elegant-border p-8 fade-in-right">
                    <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between mb-6">
                        <div>
                            <h3 class="prestige-font text-3xl font-bold mb-2">Bachelor of Commerce</h3>
                            <p class="text-xl text-gray-300">Mulund College of Commerce, Mumbai</p>
                        </div>
                        <span class="text-gray-400 text-lg tracking-wider">2021 - 2024</span>
                    </div>
                    <p class="text-gray-300 text-lg leading-relaxed mb-6">
                        Graduated with CGPA 8.0/10, building strong foundation in accounting principles, financial management, and business law. Simultaneously pursued ACCA qualification, demonstrating commitment to professional excellence.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">FINANCIAL ACCOUNTING</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">BUSINESS LAW</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">MANAGEMENT</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">ECONOMICS</span>
                    </div>
                </div>

                <div class="luxury-hover elegant-border p-8 fade-in-left">
                    <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between mb-6">
                        <div>
                            <h3 class="prestige-font text-3xl font-bold mb-2">Higher Secondary Education</h3>
                            <p class="text-xl text-gray-300">St. Xavier's English High School & Jr. College, Thane</p>
                        </div>
                        <span class="text-gray-400 text-lg tracking-wider">2019 - 2021</span>
                    </div>
                    <p class="text-gray-300 text-lg leading-relaxed mb-6">
                        Achieved 90% in HSC examinations, demonstrating academic excellence and laying the groundwork for professional accounting career. Developed strong analytical and quantitative skills.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">MATHEMATICS</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">ECONOMICS</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">ACCOUNTANCY</span>
                        <span class="elegant-border px-4 py-2 text-sm tracking-wider">BUSINESS STUDIES</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="py-24 bg-gradient-to-b from-gray-900 to-black">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="slide-up prestige-font text-5xl font-bold mb-6 tracking-wider">CORE EXPERTISE</h2>
                <div class="slide-up w-24 h-0.5 bg-white mx-auto"></div>
            </div>
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="fade-in-left">
                    <h3 class="prestige-font text-3xl font-bold mb-8 tracking-wider">TECHNICAL PROFICIENCIES</h3>
                    <div class="space-y-8">
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="text-lg font-semibold">Statutory Audit & Compliance</span>
                                <span class="text-gray-400">Advanced</span>
                            </div>
                            <div class="bg-gray-800 rounded-full h-2">
                                <div class="progress-bar h-2 rounded-full" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="text-lg font-semibold">Financial Reporting & Analysis</span>
                                <span class="text-gray-400">Advanced</span>
                            </div>
                            <div class="bg-gray-800 rounded-full h-2">
                                <div class="progress-bar h-2 rounded-full" data-width="88%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="text-lg font-semibold">Internal Controls Assessment</span>
                                <span class="text-gray-400">Proficient</span>
                            </div>
                            <div class="bg-gray-800 rounded-full h-2">
                                <div class="progress-bar h-2 rounded-full" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="text-lg font-semibold">Cost Variance Analysis</span>
                                <span class="text-gray-400">Advanced</span>
                            </div>
                            <div class="bg-gray-800 rounded-full h-2">
                                <div class="progress-bar h-2 rounded-full" data-width="87%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-3">
                                <span class="text-lg font-semibold">ACCA Standards & Frameworks</span>
                                <span class="text-gray-400">Advanced</span>
                            </div>
                            <div class="bg-gray-800 rounded-full h-2">
                                <div class="progress-bar h-2 rounded-full" data-width="92%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="fade-in-right">
                    <h3 class="prestige-font text-3xl font-bold mb-8 tracking-wider">SECTOR SPECIALIZATIONS</h3>
                    <div class="grid grid-cols-2 gap-6">
                        <div class="luxury-hover elegant-border p-6 text-center">
                            <div class="text-4xl mb-4">💊</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Pharmaceuticals</h4>
                            <p class="text-gray-400 text-sm">NIFTY 50, Large Cap</p>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-1">
                            <div class="text-4xl mb-4">🏭</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Manufacturing</h4>
                            <p class="text-gray-400 text-sm">Pre-IPO, Mid-Cap</p>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-2">
                            <div class="text-4xl mb-4">📊</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Financial Reporting</h4>
                            <p class="text-gray-400 text-sm">IFRS, Ind AS</p>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-3">
                            <div class="text-4xl mb-4">🔍</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Audit & Assurance</h4>
                            <p class="text-gray-400 text-sm">Statutory, Internal</p>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-4">
                            <div class="text-4xl mb-4">📈</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Financial Analysis</h4>
                            <p class="text-gray-400 text-sm">Variance, Performance</p>
                        </div>
                        <div class="luxury-hover elegant-border p-6 text-center stagger-5">
                            <div class="text-4xl mb-4">⚖️</div>
                            <h4 class="prestige-font text-xl font-semibold mb-2">Compliance</h4>
                            <p class="text-gray-400 text-sm">Regulatory, Standards</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Notable Achievements Section -->
    <section id="achievements" class="py-24 bg-black">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="slide-up prestige-font text-5xl font-bold mb-6 tracking-wider">KEY ACHIEVEMENTS</h2>
                <div class="slide-up w-24 h-0.5 bg-white mx-auto"></div>
            </div>
            <div class="grid lg:grid-cols-3 gap-8">
                <div class="luxury-hover elegant-border p-8 scale-in">
                    <div class="text-center mb-6">
                        <div class="text-5xl mb-4">💊</div>
                        <div class="prestige-font text-3xl font-bold mb-2">₹24,000+</div>
                        <div class="text-gray-400 text-sm tracking-wider">CRORES AUDITED</div>
                    </div>
                    <h3 class="prestige-font text-xl font-semibold mb-4">Cipla Group Audit</h3>
                    <p class="text-gray-300 mb-6">
                        Executed comprehensive statutory audit procedures for NIFTY 50 pharmaceutical giant, ensuring regulatory compliance and financial accuracy.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">NIFTY 50</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">PHARMACEUTICALS</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">STATUTORY AUDIT</span>
                    </div>
                </div>

                <div class="luxury-hover elegant-border p-8 scale-in stagger-1">
                    <div class="text-center mb-6">
                        <div class="text-5xl mb-4">📦</div>
                        <div class="prestige-font text-3xl font-bold mb-2">35%</div>
                        <div class="text-gray-400 text-sm tracking-wider">DISCREPANCY REDUCTION</div>
                    </div>
                    <h3 class="prestige-font text-xl font-semibold mb-4">Inventory Optimization</h3>
                    <p class="text-gray-300 mb-6">
                        Led inventory verification across 4 depots/plants, achieving 100% accuracy and significantly reducing reporting discrepancies.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">INVENTORY</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">VERIFICATION</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">PROCESS IMPROVEMENT</span>
                    </div>
                </div>

                <div class="luxury-hover elegant-border p-8 scale-in stagger-2">
                    <div class="text-center mb-6">
                        <div class="text-5xl mb-4">📋</div>
                        <div class="prestige-font text-3xl font-bold mb-2">100%</div>
                        <div class="text-gray-400 text-sm tracking-wider">QA COMPLIANCE</div>
                    </div>
                    <h3 class="prestige-font text-xl font-semibold mb-4">Audit Documentation</h3>
                    <p class="text-gray-300 mb-6">
                        Prepared 9+ comprehensive audit workpapers with perfect quality assurance compliance, supporting robust documentation trails.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">DOCUMENTATION</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">QUALITY ASSURANCE</span>
                        <span class="bg-gray-800 px-3 py-1 rounded text-xs tracking-wider">COMPLIANCE</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 bg-gradient-to-b from-gray-900 to-black">
        <div class="max-w-4xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="slide-up prestige-font text-5xl font-bold mb-6 tracking-wider">CONNECT</h2>
                <div class="slide-up w-24 h-0.5 bg-white mx-auto mb-8"></div>
                <p class="text-xl text-gray-300">Explore strategic opportunities and discuss your next transaction</p>
            </div>
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="fade-in-left">
                    <h3 class="prestige-font text-3xl font-bold mb-8 tracking-wider">CONTACT INFORMATION</h3>
                    <div class="space-y-8">
                        <div class="flex items-center">
                            <div class="w-16 h-16 elegant-border flex items-center justify-center mr-6">
                                <span class="text-2xl">📧</span>
                            </div>
                            <div>
                                <h4 class="prestige-font text-xl font-semibold mb-1">Email</h4>
                                <p class="text-gray-300">avandodhia.acca@gmail.com</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-16 h-16 elegant-border flex items-center justify-center mr-6">
                                <span class="text-2xl">📱</span>
                            </div>
                            <div>
                                <h4 class="prestige-font text-xl font-semibold mb-1">Phone</h4>
                                <p class="text-gray-300">+91 9004628904</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-16 h-16 elegant-border flex items-center justify-center mr-6">
                                <span class="text-2xl">📍</span>
                            </div>
                            <div>
                                <h4 class="prestige-font text-xl font-semibold mb-1">Location</h4>
                                <p class="text-gray-300">Mumbai, India</p>
                            </div>
                        </div>
                    </div>
                    <div class="mt-12">
                        <h4 class="prestige-font text-xl font-semibold mb-6 tracking-wider">PROFESSIONAL NETWORKS</h4>
                        <div class="flex space-x-6">
                            <button class="luxury-hover w-12 h-12 elegant-border flex items-center justify-center text-xl">💼</button>
                            <button class="luxury-hover w-12 h-12 elegant-border flex items-center justify-center text-xl">🌐</button>
                            <button class="luxury-hover w-12 h-12 elegant-border flex items-center justify-center text-xl">📊</button>
                        </div>
                    </div>
                </div>
                <div class="fade-in-right">
                    <form class="space-y-6" id="contact-form">
                        <div>
                            <label class="block prestige-font text-lg font-semibold mb-3 tracking-wider">NAME</label>
                            <input type="text" class="w-full px-6 py-4 bg-transparent elegant-border text-white placeholder-gray-500 focus:outline-none focus:border-white transition-colors duration-300" placeholder="Your Full Name" required>
                        </div>
                        <div>
                            <label class="block prestige-font text-lg font-semibold mb-3 tracking-wider">COMPANY</label>
                            <input type="text" class="w-full px-6 py-4 bg-transparent elegant-border text-white placeholder-gray-500 focus:outline-none focus:border-white transition-colors duration-300" placeholder="Company Name" required>
                        </div>
                        <div>
                            <label class="block prestige-font text-lg font-semibold mb-3 tracking-wider">EMAIL</label>
                            <input type="email" class="w-full px-6 py-4 bg-transparent elegant-border text-white placeholder-gray-500 focus:outline-none focus:border-white transition-colors duration-300" placeholder="your@email.com" required>
                        </div>
                        <div>
                            <label class="block prestige-font text-lg font-semibold mb-3 tracking-wider">INQUIRY TYPE</label>
                            <select class="w-full px-6 py-4 bg-black elegant-border text-white focus:outline-none focus:border-white transition-colors duration-300" required>
                                <option value="">Select Inquiry Type</option>
                                <option value="ma">M&A Advisory</option>
                                <option value="capital">Capital Markets</option>
                                <option value="strategic">Strategic Advisory</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        <div>
                            <label class="block prestige-font text-lg font-semibold mb-3 tracking-wider">MESSAGE</label>
                            <textarea rows="5" class="w-full px-6 py-4 bg-transparent elegant-border text-white placeholder-gray-500 focus:outline-none focus:border-white transition-colors duration-300" placeholder="Describe your transaction or inquiry..." required></textarea>
                        </div>
                        <button type="submit" class="luxury-hover w-full bg-white text-black py-4 prestige-font text-lg font-semibold tracking-wider transition-all duration-300">
                            SEND INQUIRY
                        </button>
                    </form>
                    <div id="form-message" class="mt-6 p-4 elegant-border hidden">
                        <p class="text-center prestige-font font-semibold"></p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black border-t border-gray-800 py-12">
        <div class="max-w-7xl mx-auto px-6 text-center">
            <p class="prestige-font text-lg tracking-wider mb-2">&copy; 2024 Avan Dodhia</p>
            <p class="text-gray-400">ACCA Trainee | Finance Professional | Audit Excellence</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
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
                    mobileMenu.classList.add('hidden');
                }
            });
        });

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate');
                }
            });
        }, observerOptions);

        // Observe all animated elements
        document.querySelectorAll('.slide-up, .fade-in-left, .fade-in-right, .scale-in').forEach(el => {
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

        document.querySelectorAll('#expertise').forEach(section => {
            progressObserver.observe(section);
        });

        // Contact form handling
        const contactForm = document.getElementById('contact-form');
        const formMessage = document.getElementById('form-message');
        
        contactForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Show success message
            formMessage.className = 'mt-6 p-4 elegant-border bg-gray-900';
            formMessage.querySelector('p').textContent = 'Thank you for your inquiry. I will respond within 24 hours.';
            formMessage.querySelector('p').className = 'text-center prestige-font font-semibold text-white';
            formMessage.classList.remove('hidden');
            
            // Reset form
            contactForm.reset();
            
            // Hide message after 5 seconds
            setTimeout(() => {
                formMessage.classList.add('hidden');
            }, 5000);
        });

        // Staggered animations for cards
        const staggerObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const staggeredElements = entry.target.querySelectorAll('[class*="stagger-"]');
                    staggeredElements.forEach((el, index) => {
                        setTimeout(() => {
                            el.classList.add('animate');
                        }, index * 100);
                    });
                }
            });
        }, observerOptions);

        document.querySelectorAll('section').forEach(section => {
            staggerObserver.observe(section);
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'96c5656b82ed3a51',t:'MTc1NDcyMzAzMy4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
