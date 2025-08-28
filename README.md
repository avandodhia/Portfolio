<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avan Dodhia - Audit Associate & ACCA Candidate</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        * {
            font-family: 'Inter', sans-serif;
        }
        
        .finance-gradient {
            background: linear-gradient(135deg, #1e3a8a 0%, #1f2937 50%, #b59f3b 100%);
        }
        
        .gold-accent {
            background: linear-gradient(135deg, #d4af37 0%, #ffd700 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }
        
        .skill-bar {
            transition: width 2s ease-in-out;
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .typing-animation {
            border-right: 2px solid #d4af37;
            animation: blink 1s infinite;
        }
        
        @keyframes blink {
            0%, 50% { border-color: #d4af37; }
            51%, 100% { border-color: transparent; }
        }
        
        .floating {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        
        .progress-circle {
            transform: rotate(-90deg);
        }
        
        .progress-circle circle {
            transition: stroke-dashoffset 2s ease-in-out;
        }
        
        .experience-timeline {
            position: relative;
        }
        
        .experience-timeline::before {
            content: '';
            position: absolute;
            left: 20px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: linear-gradient(to bottom, #d4af37, #1e3a8a);
        }
        
        .timeline-item {
            position: relative;
            padding-left: 60px;
            margin-bottom: 40px;
        }
        
        .timeline-dot {
            position: absolute;
            left: 11px;
            top: 8px;
            width: 18px;
            height: 18px;
            border-radius: 50%;
            background: #d4af37;
            border: 3px solid white;
            box-shadow: 0 0 0 3px #d4af37;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-white/95 backdrop-blur-md z-50 shadow-sm border-b border-gray-100">
        <div class="max-w-6xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold text-gray-800">
                    <span class="text-blue-900">Avan</span> <span class="gold-accent bg-clip-text text-transparent">Dodhia</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">Home</a>
                    <a href="#about" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">About</a>
                    <a href="#experience" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">Experience</a>
                    <a href="#skills" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">Skills</a>
                    <a href="#education" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">Education</a>
                    <a href="#contact" class="text-gray-700 hover:text-blue-900 transition-colors font-medium">Contact</a>
                </div>
                <button id="mobile-menu" class="md:hidden">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen finance-gradient flex items-center justify-center text-white">
        <div class="max-w-5xl mx-auto px-6 text-center">
            <div class="floating mb-8">
                <div class="w-40 h-40 mx-auto rounded-full bg-white/10 backdrop-blur-md flex items-center justify-center text-7xl border-4 border-white/20">
                    📊
                </div>
            </div>
            <h1 class="text-5xl md:text-7xl font-bold mb-6 fade-in">
                <span class="typing-animation">Avan Dodhia</span>
            </h1>
            <p class="text-2xl md:text-3xl mb-4 fade-in font-light">
                Audit Associate | ACCA Candidate
            </p>
            <p class="text-xl mb-8 fade-in opacity-90 font-light">
                Aspiring Investment Banking Analyst
            </p>
            <p class="text-lg mb-12 fade-in opacity-80 max-w-3xl mx-auto leading-relaxed">
                Experienced in financial auditing with expertise in IFRS, cost analysis, and stakeholder management. 
                Currently pursuing ACCA Professional Level with a passion for investment banking and financial markets.
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center fade-in">
                <a href="#experience" class="bg-white text-blue-900 px-8 py-4 rounded-full font-semibold hover:bg-gray-100 transition-colors shadow-lg">
                    View Experience
                </a>
                <a href="#contact" class="border-2 border-white text-white px-8 py-4 rounded-full font-semibold hover:bg-white hover:text-blue-900 transition-colors">
                    Get In Touch
                </a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">About Me</h2>
                <div class="w-20 h-1 gold-accent mx-auto rounded"></div>
            </div>
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="fade-in">
                    <div class="w-80 h-80 mx-auto rounded-2xl finance-gradient flex items-center justify-center text-8xl text-white shadow-2xl">
                        💼
                    </div>
                </div>
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Finance Professional & Analytical Thinker</h3>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        As an Audit Associate at Grant Thornton Bharat LLP, I've had the privilege of working with 
                        large-scale clients including Cipla (₹24,000+ Cr revenue) and IPO-preparing firms. My experience 
                        spans financial auditing, cost variance analysis, and stakeholder management.
                    </p>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        Currently pursuing ACCA Professional Level (11/13 papers cleared), I'm passionate about 
                        transitioning into investment banking where I can leverage my analytical skills and 
                        financial expertise to drive strategic decision-making.
                    </p>
                    <p class="text-gray-600 mb-8 leading-relaxed">
                        Beyond finance, I enjoy reading business literature, playing football, and beatboxing - 
                        activities that keep me balanced and creative.
                    </p>
                    <div class="flex flex-wrap gap-3">
                        <span class="bg-blue-100 text-blue-800 px-4 py-2 rounded-full text-sm font-medium">Financial Analysis</span>
                        <span class="bg-yellow-100 text-yellow-800 px-4 py-2 rounded-full text-sm font-medium">ACCA Candidate</span>
                        <span class="bg-green-100 text-green-800 px-4 py-2 rounded-full text-sm font-medium">Audit Expert</span>
                        <span class="bg-purple-100 text-purple-800 px-4 py-2 rounded-full text-sm font-medium">IB Aspirant</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Professional Experience</h2>
                <div class="w-20 h-1 gold-accent mx-auto rounded"></div>
            </div>
            
            <div class="experience-timeline fade-in">
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="bg-white rounded-xl p-8 shadow-lg card-hover">
                        <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-4">
                            <h3 class="text-2xl font-bold text-gray-800">Audit Associate</h3>
                            <span class="text-blue-600 font-semibold bg-blue-50 px-4 py-2 rounded-full">July 2024 – Feb 2025</span>
                        </div>
                        <h4 class="text-xl text-gray-600 mb-6 font-medium">Grant Thornton Bharat LLP – Mumbai</h4>
                        
                        <div class="grid md:grid-cols-2 gap-6">
                            <div>
                                <h5 class="font-semibold text-gray-800 mb-3 flex items-center">
                                    <span class="w-2 h-2 gold-accent rounded-full mr-3"></span>
                                    Key Achievements
                                </h5>
                                <ul class="space-y-2 text-gray-600">
                                    <li class="flex items-start">
                                        <span class="text-green-500 mr-2 mt-1">✓</span>
                                        Audited large clients: Cipla (₹24,000+ Cr revenue)
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-green-500 mr-2 mt-1">✓</span>
                                        Led inventory verification at 4 depots/plants
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-green-500 mr-2 mt-1">✓</span>
                                        Reduced discrepancies by 35%
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-green-500 mr-2 mt-1">✓</span>
                                        Created 9+ audit workpapers with 100% QA compliance
                                    </li>
                                </ul>
                            </div>
                            <div>
                                <h5 class="font-semibold text-gray-800 mb-3 flex items-center">
                                    <span class="w-2 h-2 gold-accent rounded-full mr-3"></span>
                                    Impact & Results
                                </h5>
                                <ul class="space-y-2 text-gray-600">
                                    <li class="flex items-start">
                                        <span class="text-blue-500 mr-2 mt-1">📊</span>
                                        Cost variance analysis across 5+ OpEx categories
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-blue-500 mr-2 mt-1">📋</span>
                                        Prepared reports for 12+ stakeholders
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-blue-500 mr-2 mt-1">🚀</span>
                                        20% boost in audit readiness through improvements
                                    </li>
                                    <li class="flex items-start">
                                        <span class="text-blue-500 mr-2 mt-1">🎯</span>
                                        IPO-preparing firm audit (₹500+ Cr revenue)
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Projects Section -->
            <div class="mt-16 fade-in">
                <h3 class="text-2xl font-bold text-gray-800 mb-8 text-center">Key Projects & Activities</h3>
                <div class="grid md:grid-cols-3 gap-6">
                    <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                        <div class="text-4xl mb-4 text-center">🏭</div>
                        <h4 class="text-lg font-semibold text-gray-800 mb-3">Financial Audits</h4>
                        <p class="text-gray-600 text-sm">Statutory audits for listed pharmaceutical companies and IPO-preparing manufacturing firms with comprehensive compliance frameworks.</p>
                    </div>
                    <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                        <div class="text-4xl mb-4 text-center">⚙️</div>
                        <h4 class="text-lg font-semibold text-gray-800 mb-3">Process Improvements</h4>
                        <p class="text-gray-600 text-sm">Identified gaps in compliance frameworks and implemented solutions that improved audit alignment and operational efficiency.</p>
                    </div>
                    <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                        <div class="text-4xl mb-4 text-center">🎯</div>
                        <h4 class="text-lg font-semibold text-gray-800 mb-3">Leadership & Events</h4>
                        <p class="text-gray-600 text-sm">Managed logistics, troubleshooting, registrations, and social media outreach for college events, demonstrating strong organizational skills.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Skills & Expertise</h2>
                <div class="w-20 h-1 gold-accent mx-auto rounded"></div>
            </div>
            
            <div class="grid lg:grid-cols-3 gap-12">
                <!-- Technical Skills -->
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-8 text-center">Technical Skills</h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700 font-medium">Financial Analysis</span>
                                <span class="text-gray-500">95%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-3">
                                <div class="skill-bar bg-gradient-to-r from-blue-600 to-blue-800 h-3 rounded-full" style="width: 0%" data-width="95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700 font-medium">IFRS & Ind AS</span>
                                <span class="text-gray-500">90%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-3">
                                <div class="skill-bar bg-gradient-to-r from-yellow-500 to-yellow-600 h-3 rounded-full" style="width: 0%" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700 font-medium">Audit Documentation</span>
                                <span class="text-gray-500">92%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-3">
                                <div class="skill-bar bg-gradient-to-r from-green-500 to-green-600 h-3 rounded-full" style="width: 0%" data-width="92%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700 font-medium">Microsoft Office Suite</span>
                                <span class="text-gray-500">88%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-3">
                                <div class="skill-bar bg-gradient-to-r from-purple-500 to-purple-600 h-3 rounded-full" style="width: 0%" data-width="88%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700 font-medium">Cost Variance Analysis</span>
                                <span class="text-gray-500">85%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-3">
                                <div class="skill-bar bg-gradient-to-r from-red-500 to-red-600 h-3 rounded-full" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Soft Skills -->
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-8 text-center">Soft Skills</h3>
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">👥</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Leadership</h4>
                        </div>
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">🧠</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Business Acumen</h4>
                        </div>
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">🔍</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Analytical Thinking</h4>
                        </div>
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">🎯</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Problem Solving</h4>
                        </div>
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">💬</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Communication</h4>
                        </div>
                        <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
                            <div class="text-4xl mb-3">🤝</div>
                            <h4 class="font-semibold text-gray-800 text-sm">Stakeholder Mgmt</h4>
                        </div>
                    </div>
                </div>

                <!-- Languages -->
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-8 text-center">Languages</h3>
                    <div class="space-y-6">
                        <div class="flex items-center justify-between p-4 bg-gray-50 rounded-lg">
                            <div class="flex items-center">
                                <span class="text-2xl mr-3">🇬🇧</span>
                                <span class="font-medium text-gray-800">English</span>
                            </div>
                            <span class="text-green-600 font-semibold">Fluent</span>
                        </div>
                        <div class="flex items-center justify-between p-4 bg-gray-50 rounded-lg">
                            <div class="flex items-center">
                                <span class="text-2xl mr-3">🇮🇳</span>
                                <span class="font-medium text-gray-800">Hindi</span>
                            </div>
                            <span class="text-green-600 font-semibold">Native</span>
                        </div>
                        <div class="flex items-center justify-between p-4 bg-gray-50 rounded-lg">
                            <div class="flex items-center">
                                <span class="text-2xl mr-3">🇮🇳</span>
                                <span class="font-medium text-gray-800">Gujarati</span>
                            </div>
                            <span class="text-green-600 font-semibold">Native</span>
                        </div>
                        <div class="flex items-center justify-between p-4 bg-gray-50 rounded-lg">
                            <div class="flex items-center">
                                <span class="text-2xl mr-3">🇮🇳</span>
                                <span class="font-medium text-gray-800">Marathi</span>
                            </div>
                            <span class="text-blue-600 font-semibold">Proficient</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Education & Certifications</h2>
                <div class="w-20 h-1 gold-accent mx-auto rounded"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-8">
                <!-- Education -->
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-8">Education</h3>
                    <div class="space-y-6">
                        <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                            <div class="flex items-center mb-4">
                                <div class="w-16 h-16 finance-gradient rounded-full flex items-center justify-center text-white text-2xl mr-4">
                                    🎓
                                </div>
                                <div>
                                    <h4 class="text-lg font-semibold text-gray-800">ACCA (Professional Level)</h4>
                                    <p class="text-gray-600">11/13 Papers Cleared</p>
                                    <p class="text-sm text-blue-600 font-medium">Ongoing</p>
                                </div>
                            </div>
                            <div class="bg-gray-50 rounded-lg p-4">
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-sm font-medium text-gray-700">Progress</span>
                                    <span class="text-sm font-medium text-gray-700">85%</span>
                                </div>
                                <div class="bg-gray-200 rounded-full h-2">
                                    <div class="bg-gradient-to-r from-blue-500 to-green-500 h-2 rounded-full" style="width: 85%"></div>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                            <div class="flex items-center mb-4">
                                <div class="w-16 h-16 bg-green-600 rounded-full flex items-center justify-center text-white text-2xl mr-4">
                                    📚
                                </div>
                                <div>
                                    <h4 class="text-lg font-semibold text-gray-800">B.Com</h4>
                                    <p class="text-gray-600">Mulund College of Commerce</p>
                                    <p class="text-sm text-green-600 font-medium">8.0 CGPA (2021–24)</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                            <div class="flex items-center mb-4">
                                <div class="w-16 h-16 bg-purple-600 rounded-full flex items-center justify-center text-white text-2xl mr-4">
                                    🏫
                                </div>
                                <div>
                                    <h4 class="text-lg font-semibold text-gray-800">HSC</h4>
                                    <p class="text-gray-600">St. Xavier's English High School</p>
                                    <p class="text-sm text-purple-600 font-medium">90%</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Certifications -->
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-8">Certifications</h3>
                    <div class="space-y-6">
                        <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                            <div class="flex items-center mb-4">
                                <div class="w-16 h-16 gold-accent rounded-full flex items-center justify-center text-white text-2xl mr-4">
                                    🏆
                                </div>
                                <div>
                                    <h4 class="text-lg font-semibold text-gray-800">ACCA Advanced Diploma</h4>
                                    <p class="text-gray-600">Accounting and Business</p>
                                    <p class="text-sm text-yellow-600 font-medium">Professional Qualification</p>
                                </div>
                            </div>
                            <p class="text-gray-600 text-sm">Comprehensive understanding of financial reporting, management accounting, and business strategy.</p>
                        </div>

                        <div class="bg-white rounded-xl p-6 shadow-lg card-hover">
                            <div class="flex items-center mb-4">
                                <div class="w-16 h-16 bg-blue-600 rounded-full flex items-center justify-center text-white text-2xl mr-4">
                                    🏛️
                                </div>
                                <div>
                                    <h4 class="text-lg font-semibold text-gray-800">Goldman Sachs</h4>
                                    <p class="text-gray-600">Risk Management Virtual Internship</p>
                                    <p class="text-sm text-blue-600 font-medium">Forage Platform</p>
                                </div>
                            </div>
                            <p class="text-gray-600 text-sm">Gained insights into investment banking risk management practices and financial modeling techniques.</p>
                        </div>

                        <!-- Interests -->
                        <div class="bg-white rounded-xl p-6 shadow-lg">
                            <h4 class="text-lg font-semibold text-gray-800 mb-4">Interests & Hobbies</h4>
                            <div class="flex flex-wrap gap-3">
                                <div class="flex items-center bg-gray-50 px-4 py-2 rounded-full">
                                    <span class="text-xl mr-2">📖</span>
                                    <span class="text-sm font-medium text-gray-700">Business Reading</span>
                                </div>
                                <div class="flex items-center bg-gray-50 px-4 py-2 rounded-full">
                                    <span class="text-xl mr-2">⚽</span>
                                    <span class="text-sm font-medium text-gray-700">Football</span>
                                </div>
                                <div class="flex items-center bg-gray-50 px-4 py-2 rounded-full">
                                    <span class="text-xl mr-2">🎵</span>
                                    <span class="text-sm font-medium text-gray-700">Beatboxing</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 finance-gradient text-white">
        <div class="max-w-4xl mx-auto px-6">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold mb-4">Let's Connect</h2>
                <div class="w-20 h-1 bg-white mx-auto rounded"></div>
                <p class="text-xl mt-4 opacity-90">Ready to discuss opportunities in finance and investment banking</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12">
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold mb-6">Contact Information</h3>
                    <div class="space-y-6">
                        <div class="flex items-center space-x-4">
                            <div class="w-14 h-14 bg-white/20 rounded-full flex items-center justify-center text-2xl">
                                📧
                            </div>
                            <div>
                                <p class="font-medium text-lg">Email</p>
                                <p class="opacity-80">avandodhia.acca@gmail.com</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-14 h-14 bg-white/20 rounded-full flex items-center justify-center text-2xl">
                                📱
                            </div>
                            <div>
                                <p class="font-medium text-lg">Phone</p>
                                <p class="opacity-80">+91 9004628904</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-14 h-14 bg-white/20 rounded-full flex items-center justify-center text-2xl">
                                💼
                            </div>
                            <div>
                                <p class="font-medium text-lg">LinkedIn</p>
                                <p class="opacity-80">linkedin.com/in/avan-dodhia</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-14 h-14 bg-white/20 rounded-full flex items-center justify-center text-2xl">
                                📍
                            </div>
                            <div>
                                <p class="font-medium text-lg">Location</p>
                                <p class="opacity-80">Mumbai, India</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="fade-in">
                    <form id="contact-form" class="space-y-6">
                        <div>
                            <input type="text" placeholder="Your Name" required 
                                   class="w-full px-4 py-3 rounded-lg bg-white/10 border border-white/20 text-white placeholder-white/70 focus:outline-none focus:border-white/50 focus:bg-white/20">
                        </div>
                        <div>
                            <input type="email" placeholder="Your Email" required 
                                   class="w-full px-4 py-3 rounded-lg bg-white/10 border border-white/20 text-white placeholder-white/70 focus:outline-none focus:border-white/50 focus:bg-white/20">
                        </div>
                        <div>
                            <input type="text" placeholder="Subject" required 
                                   class="w-full px-4 py-3 rounded-lg bg-white/10 border border-white/20 text-white placeholder-white/70 focus:outline-none focus:border-white/50 focus:bg-white/20">
                        </div>
                        <div>
                            <textarea placeholder="Your Message" rows="4" required 
                                      class="w-full px-4 py-3 rounded-lg bg-white/10 border border-white/20 text-white placeholder-white/70 focus:outline-none focus:border-white/50 focus:bg-white/20 resize-none"></textarea>
                        </div>
                        <button type="submit" 
                                class="w-full bg-white text-blue-900 py-3 rounded-lg font-semibold hover:bg-gray-100 transition-colors shadow-lg">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center">
                <div class="text-2xl font-bold mb-4">
                    <span class="text-blue-400">Avan</span> <span class="gold-accent bg-clip-text text-transparent">Dodhia</span>
                </div>
                <p class="text-gray-400 mb-6">Audit Associate | ACCA Candidate | Aspiring Investment Banking Analyst</p>
                <div class="flex justify-center space-x-6 mb-8">
                    <a href="mailto:avandodhia.acca@gmail.com" class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center hover:bg-blue-600 transition-colors">
                        📧
                    </a>
                    <a href="https://linkedin.com/in/avan-dodhia" target="_blank" class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center hover:bg-blue-600 transition-colors">
                        💼
                    </a>
                    <a href="tel:+919004628904" class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center hover:bg-blue-600 transition-colors">
                        📱
                    </a>
                </div>
                <div class="border-t border-gray-800 pt-8">
                    <p class="text-gray-400">© 2024 Avan Dodhia. All rights reserved.</p>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
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

        // Fade in animation on scroll
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

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Skill bar animation
        const skillObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const skillBars = entry.target.querySelectorAll('.skill-bar');
                    skillBars.forEach(bar => {
                        const width = bar.getAttribute('data-width');
                        setTimeout(() => {
                            bar.style.width = width;
                        }, 500);
                    });
                }
            });
        }, { threshold: 0.5 });

        const skillsSection = document.querySelector('#skills');
        if (skillsSection) {
            skillObserver.observe(skillsSection);
        }

        // Typing animation
        const typingElement = document.querySelector('.typing-animation');
        if (typingElement) {
            const text = 'Avan Dodhia';
            let index = 0;
            
            function typeText() {
                if (index < text.length) {
                    typingElement.textContent = text.slice(0, index + 1);
                    index++;
                    setTimeout(typeText, 150);
                }
            }
            
            setTimeout(typeText, 1000);
        }

        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu');
        
        mobileMenuBtn?.addEventListener('click', () => {
            alert('Mobile menu would open here. This portfolio is optimized for desktop viewing for professional purposes.');
        });

        // Contact form submission
        document.getElementById('contact-form')?.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const name = this.querySelector('input[type="text"]').value;
            const email = this.querySelector('input[type="email"]').value;
            const subject = this.querySelectorAll('input[type="text"]')[1].value;
            const message = this.querySelector('textarea').value;
            
            if (name && email && subject && message) {
                const button = this.querySelector('button[type="submit"]');
                const originalText = button.textContent;
                
                button.textContent = 'Sending...';
                button.disabled = true;
                
                setTimeout(() => {
                    alert(`Thank you ${name}! Your message regarding "${subject}" has been received. I'll respond within 24 hours to discuss potential opportunities.`);
                    this.reset();
                    button.textContent = originalText;
                    button.disabled = false;
                }, 1500);
            }
        });

        // Add some initial animations
        window.addEventListener('load', () => {
            document.querySelectorAll('.fade-in').forEach(el => {
                const rect = el.getBoundingClientRect();
                if (rect.top < window.innerHeight) {
                    el.classList.add('visible');
                }
            });
        });

        // Professional interactions
        document.querySelectorAll('.card-hover').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-8px)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9761e5abb5e985d1',t:'MTc1NjM2NDA2NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
