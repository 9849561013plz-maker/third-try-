<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ChannelDoctor Pro - Free AI Channel Audit & Growth Analysis</title>
    <meta name="description" content="Get a free AI-powered channel audit in 30 seconds. Fix hidden mistakes killing your YouTube & TikTok growth with personalized 7-day action plans.">
    
    <!-- Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'GA_MEASUREMENT_ID');
    </script>
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        * {
            font-family: 'Inter', sans-serif;
            box-sizing: border-box;
        }
        h1, h2, h3, .brand-font {
            font-family: 'Space Grotesk', sans-serif;
        }
        
        /* Animated Background */
        .gradient-bg {
            background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
        }
        
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        /* Glassmorphism */
        .glass {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .glass-dark {
            background: rgba(17, 24, 39, 0.8);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        /* Pulse Animation */
        .pulse-ring {
            animation: pulse-ring 2s cubic-bezier(0.215, 0.61, 0.355, 1) infinite;
        }
        
        @keyframes pulse-ring {
            0% { transform: scale(0.8); opacity: 0.8; }
            100% { transform: scale(2); opacity: 0; }
        }
        
        /* Floating Elements */
        .float {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        /* Progress Bar Animation */
        .progress-fill {
            transition: width 1s ease-out;
        }
        
        /* Card Hover Effects */
        .hover-card {
            transition: all 0.3s ease;
        }
        .hover-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }
        
        /* Score Ring Animation */
        .score-ring {
            transition: stroke-dashoffset 1s ease-in-out, stroke 0.5s ease;
        }

        /* Modal Animation */
        .modal-enter {
            animation: modalEnter 0.3s ease-out;
        }
        @keyframes modalEnter {
            from { opacity: 0; transform: scale(0.95); }
            to { opacity: 1; transform: scale(1); }
        }

        /* Day Plan Card */
        .day-card {
            background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(236, 72, 153, 0.1) 100%);
            border: 1px solid rgba(139, 92, 246, 0.3);
            transition: all 0.3s ease;
        }
        .day-card:hover {
            transform: translateY(-3px);
            border-color: rgba(139, 92, 246, 0.6);
            box-shadow: 0 10px 30px rgba(139, 92, 246, 0.2);
        }
        .day-card.completed {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1) 0%, rgba(5, 150, 105, 0.1) 100%);
            border-color: rgba(16, 185, 129, 0.3);
        }

        /* Severity Colors */
        .severity-critical { border-left: 4px solid #ef4444; }
        .severity-warning { border-left: 4px solid #f59e0b; }
        .severity-info { border-left: 4px solid #3b82f6; }
        .severity-success { border-left: 4px solid #10b981; }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #1f2937;
        }
        ::-webkit-scrollbar-thumb {
            background: #4b5563;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #6b7280;
        }

        /* Button Hover Effects */
        .btn-primary {
            background: linear-gradient(135deg, #9333ea 0%, #db2777 100%);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(147, 51, 234, 0.4);
        }
        .btn-primary:active {
            transform: translateY(0);
        }
        .btn-primary::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.3), transparent);
            transform: rotate(45deg);
            transition: all 0.5s;
            opacity: 0;
        }
        .btn-primary:hover::after {
            opacity: 1;
            left: 100%;
        }

        /* Score Colors */
        .score-high { color: #10b981; }
        .score-medium { color: #f59e0b; }
        .score-low { color: #ef4444; }

        /* Testimonial Card */
        .testimonial-card {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        .testimonial-card:hover {
            background: rgba(255, 255, 255, 0.08);
            transform: translateY(-5px);
        }

        /* Mobile Optimizations */
        @media (max-width: 640px) {
            .hero-title {
                font-size: 2.5rem !important;
                line-height: 1.2 !important;
            }
            .glass-dark {
                backdrop-filter: blur(8px);
            }
        }

        /* Loading Skeleton */
        .skeleton {
            background: linear-gradient(90deg, #374151 25%, #4b5563 50%, #374151 75%);
            background-size: 200% 100%;
            animation: skeleton 1.5s infinite;
        }
        @keyframes skeleton {
            0% { background-position: 200% 0; }
            100% { background-position: -200% 0; }
        }

        /* Feedback Button */
        .feedback-btn {
            position: fixed;
            bottom: 20px;
            left: 20px;
            z-index: 40;
            background: rgba(17, 24, 39, 0.9);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="bg-gray-900 text-white min-h-screen overflow-x-hidden">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass-dark border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center space-x-2 cursor-pointer" onclick="scrollToTop()">
                    <div class="relative">
                        <div class="w-10 h-10 bg-gradient-to-br from-purple-500 to-pink-500 rounded-lg flex items-center justify-center">
                            <i class="fas fa-stethoscope text-white text-xl"></i>
                        </div>
                        <div class="absolute -top-1 -right-1 w-3 h-3 bg-green-400 rounded-full pulse-ring"></div>
                    </div>
                    <span class="brand-font text-2xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-purple-400 to-pink-400">
                        ChannelDoctor
                    </span>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#features" class="text-gray-300 hover:text-white transition text-sm font-medium">Features</a>
                    <a href="#how-it-works" class="text-gray-300 hover:text-white transition text-sm font-medium">How It Works</a>
                    <a href="#testimonials" class="text-gray-300 hover:text-white transition text-sm font-medium">Reviews</a>
                    <button onclick="scrollToTop()" class="btn-primary px-6 py-2.5 rounded-full font-semibold text-sm">
                        Get Free Audit
                    </button>
                </div>
                <button class="md:hidden text-white p-2" onclick="toggleMobileMenu()" aria-label="Toggle menu">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobileMenu" class="hidden md:hidden glass-dark border-t border-gray-800">
            <div class="px-4 py-4 space-y-3">
                <a href="#features" class="block text-gray-300 hover:text-white py-2">Features</a>
                <a href="#how-it-works" class="block text-gray-300 hover:text-white py-2">How It Works</a>
                <a href="#testimonials" class="block text-gray-300 hover:text-white py-2">Reviews</a>
                <button onclick="scrollToTop()" class="w-full btn-primary px-6 py-3 rounded-full font-semibold mt-2">
                    Get Free Audit
                </button>
            </div>
        </div>
    </nav>

    <!-- Trust Badge (Fixed) -->
    <div class="fixed bottom-4 right-4 z-40 hidden md:flex items-center gap-2 glass-dark px-4 py-2 rounded-full border border-gray-700 text-sm shadow-lg">
        <i class="fas fa-shield-alt text-green-400"></i>
        <span class="text-gray-300">Trusted by 50,000+ creators</span>
    </div>

    <!-- Hero Section - Above Fold -->
    <section class="relative pt-28 pb-16 md:pt-32 md:pb-20 overflow-hidden min-h-screen flex items-center">
        <div class="absolute inset-0 gradient-bg opacity-20"></div>
        <div class="absolute inset-0 bg-[url('data:image/svg+xml,%3Csvg width=\'60\' height=\'60\' viewBox=\'0 0 60 60\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cg fill=\'none\' fill-rule=\'evenodd\'%3E%3Cg fill=\'%239C92AC\' fill-opacity=\'0.05\'%3E%3Cpath d=\'M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z\'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E')]"></div>
        
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full">
            <div class="grid lg:grid-cols-2 gap-12 items-center">
                <!-- Left: Content -->
                <div class="text-center lg:text-left">
                    <!-- Trust Banner -->
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-blue-500/10 border border-blue-500/30 text-blue-300 text-sm mb-6 animate-pulse">
                        <i class="fas fa-check-circle"></i>
                        <span>100% Free • No Credit Card Required</span>
                    </div>
                    
                    <h1 class="hero-title text-4xl md:text-6xl lg:text-7xl font-bold mb-6 leading-tight">
                        Fix Your Channel's<br>
                        <span class="bg-clip-text text-transparent bg-gradient-to-r from-red-400 via-pink-400 to-purple-400">
                            Growth Problems
                        </span><br>
                        <span class="text-2xl md:text-4xl font-normal text-gray-400">in 30 Seconds</span>
                    </h1>
                    
                    <p class="text-lg md:text-xl text-gray-400 max-w-2xl mx-auto lg:mx-0 mb-8 leading-relaxed">
                        Paste your YouTube or TikTok link to get a <span class="text-white font-semibold">free AI-powered audit</span>. 
                        Discover hidden mistakes killing your reach and get a personalized 7-day growth plan.
                    </p>

                    <!-- 3-Step Visual -->
                    <div class="flex flex-wrap justify-center lg:justify-start gap-4 mb-8 text-sm text-gray-400">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 rounded-full bg-purple-500/20 flex items-center justify-center text-purple-400 font-bold border border-purple-500/30">1</div>
                            <span>Paste URL</span>
                        </div>
                        <i class="fas fa-arrow-right text-gray-600 hidden sm:block self-center"></i>
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 rounded-full bg-pink-500/20 flex items-center justify-center text-pink-400 font-bold border border-pink-500/30">2</div>
                            <span>AI Analyzes</span>
                        </div>
                        <i class="fas fa-arrow-right text-gray-600 hidden sm:block self-center"></i>
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 rounded-full bg-green-500/20 flex items-center justify-center text-green-400 font-bold border border-green-500/30">3</div>
                            <span>Get Fix Plan</span>
                        </div>
                    </div>

                    <!-- Main Input Section -->
                    <div class="max-w-xl mx-auto lg:mx-0">
                        <div class="glass rounded-2xl p-2 shadow-2xl shadow-purple-500/20 border border-gray-700">
                            <div class="flex flex-col sm:flex-row gap-2">
                                <div class="flex-1 relative">
                                    <i class="fas fa-link absolute left-4 top-1/2 transform -translate-y-1/2 text-gray-400"></i>
                                    <input 
                                        type="url" 
                                        id="channelUrl" 
                                        placeholder="Paste YouTube or TikTok channel URL..."
                                        class="w-full pl-12 pr-4 py-4 bg-gray-800/50 border border-gray-700 rounded-xl text-white placeholder-gray-500 focus:outline-none focus:border-purple-500 focus:ring-2 focus:ring-purple-500/20 transition text-base"
                                        aria-label="Channel URL input"
                                    >
                                </div>
                                <button 
                                    onclick="startAnalysis()"
                                    id="analyzeBtn"
                                    class="btn-primary px-6 py-4 rounded-xl font-bold text-base sm:text-lg whitespace-nowrap flex items-center justify-center gap-2 min-w-[180px]"
                                >
                                    <span>Analyze Now</span>
                                    <i class="fas fa-arrow-right"></i>
                                </button>
                            </div>
                        </div>
                        
                        <!-- Platform Icons -->
                        <div class="flex justify-center lg:justify-start gap-6 mt-4 text-gray-500">
                            <div class="flex flex-col items-center gap-1 group cursor-pointer hover:text-red-500 transition" onclick="fillExample('youtube')">
                                <i class="fab fa-youtube text-2xl"></i>
                                <span class="text-xs">YouTube</span>
                            </div>
                            <div class="flex flex-col items-center gap-1 group cursor-pointer hover:text-cyan-400 transition" onclick="fillExample('tiktok')">
                                <i class="fab fa-tiktok text-2xl"></i>
                                <span class="text-xs">TikTok</span>
                            </div>
                            <div class="flex flex-col items-center gap-1 opacity-50">
                                <i class="fab fa-instagram text-2xl"></i>
                                <span class="text-xs">Soon</span>
                            </div>
                        </div>

                        <!-- See Example Report -->
                        <div class="mt-4">
                            <button onclick="showDemoReport()" class="text-purple-400 hover:text-purple-300 text-sm font-medium flex items-center gap-2 mx-auto lg:mx-0 hover:underline decoration-dotted underline-offset-4">
                                <i class="fas fa-play-circle"></i>
                                See Example Report First
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Right: Stats & Social Proof -->
                <div class="hidden lg:block">
                    <div class="glass-dark rounded-3xl p-8 border border-gray-700 relative overflow-hidden">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-purple-500/20 rounded-full blur-3xl"></div>
                        
                        <!-- Live Stats -->
                        <div class="grid grid-cols-2 gap-6 mb-8">
                            <div class="text-center p-4 rounded-2xl bg-gray-800/50 border border-gray-700">
                                <div class="text-3xl font-bold text-purple-400 mb-1">50K+</div>
                                <div class="text-sm text-gray-500">Channels Analyzed</div>
                            </div>
                            <div class="text-center p-4 rounded-2xl bg-gray-800/50 border border-gray-700">
                                <div class="text-3xl font-bold text-green-400 mb-1">94%</div>
                                <div class="text-sm text-gray-500">See Growth in 7 Days</div>
                            </div>
                            <div class="text-center p-4 rounded-2xl bg-gray-800/50 border border-gray-700">
                                <div class="text-3xl font-bold text-pink-400 mb-1">12</div>
                                <div class="text-sm text-gray-500">Issues Detected Avg</div>
                            </div>
                            <div class="text-center p-4 rounded-2xl bg-gray-800/50 border border-gray-700">
                                <div class="text-3xl font-bold text-blue-400 mb-1">100%</div>
                                <div class="text-sm text-gray-500">Free Forever</div>
                            </div>
                        </div>

                        <!-- Mini Testimonial -->
                        <div class="bg-gray-800/30 rounded-xl p-4 border border-gray-700">
                            <div class="flex items-start gap-3">
                                <div class="w-10 h-10 rounded-full bg-gradient-to-br from-purple-500 to-pink-500 flex items-center justify-center text-sm font-bold">JD</div>
                                <div>
                                    <p class="text-sm text-gray-300 mb-2">"Found 8 critical issues I never knew existed. Fixed them and gained 2K subs in a week!"</p>
                                    <div class="flex items-center gap-2 text-xs text-gray-500">
                                        <span class="text-yellow-400">★★★★★</span>
                                        <span>•</span>
                                        <span>@TechCreator_Pro</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Demo Report Modal -->
    <div id="demoModal" class="hidden fixed inset-0 bg-black/90 z-50 flex items-center justify-center p-4 backdrop-blur-sm overflow-y-auto">
        <div class="glass-dark rounded-3xl max-w-4xl w-full max-h-[90vh] overflow-y-auto modal-enter border border-gray-700 shadow-2xl">
            <div class="sticky top-0 bg-gray-900/95 backdrop-blur border-b border-gray-800 p-6 flex justify-between items-center z-10">
                <div>
                    <h3 class="text-2xl font-bold brand-font">Example Report: TechCreator_Pro</h3>
                    <p class="text-gray-400 text-sm mt-1">YouTube Channel • 12.5K Subscribers • <span class="text-yellow-400">Demo Mode</span></p>
                </div>
                <button onclick="closeDemoReport()" class="w-10 h-10 rounded-full bg-gray-800 hover:bg-gray-700 flex items-center justify-center transition" aria-label="Close modal">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            
            <div class="p-6 space-y-6">
                <!-- Demo Score -->
                <div class="glass-dark rounded-2xl p-6 flex flex-col md:flex-row items-center gap-6 border border-gray-700">
                    <div class="relative">
                        <svg class="w-32 h-32 transform -rotate-90">
                            <circle cx="64" cy="64" r="56" stroke="#374151" stroke-width="10" fill="none"/>
                            <circle cx="64" cy="64" r="56" stroke="#f59e0b" stroke-width="10" fill="none" 
                                stroke-dasharray="351" stroke-dashoffset="105" stroke-linecap="round"/>
                        </svg>
                        <div class="absolute inset-0 flex items-center justify-center flex-col">
                            <span class="text-3xl font-bold">70</span>
                            <span class="text-xs text-gray-500">Health Score</span>
                        </div>
                    </div>
                    <div class="flex-1 text-center md:text-left">
                        <h4 class="text-xl font-bold text-yellow-400 mb-2">Needs Improvement</h4>
                        <p class="text-gray-400 mb-4">Good foundation, but 5 critical issues are limiting growth potential. Estimated <span class="text-green-400 font-semibold">+3,200 monthly subscribers</span> if fixed.</p>
                        <div class="flex gap-2 flex-wrap justify-center md:justify-start">
                            <span class="px-3 py-1 rounded-full bg-red-500/20 text-red-400 text-xs border border-red-500/30">5 Critical</span>
                            <span class="px-3 py-1 rounded-full bg-yellow-500/20 text-yellow-400 text-xs border border-yellow-500/30">3 Warnings</span>
                            <span class="px-3 py-1 rounded-full bg-blue-500/20 text-blue-400 text-xs border border-blue-500/30">2 Suggestions</span>
                        </div>
                    </div>
                </div>

                <!-- Demo Detected Problems -->
                <div class="bg-red-500/10 border border-red-500/30 rounded-2xl p-6">
                    <h4 class="text-lg font-bold text-red-400 mb-4 flex items-center gap-2">
                        <i class="fas fa-exclamation-triangle"></i>
                        Critical Issues Found
                    </h4>
                    <ul class="space-y-3 text-gray-300">
                        <li class="flex items-start gap-3">
                            <i class="fas fa-times-circle text-red-400 mt-1"></i>
                            <span>Upload frequency too low (1 video/month vs recommended 4)</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fas fa-times-circle text-red-400 mt-1"></i>
                            <span>Weak video titles - no curiosity gap or emotional trigger</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fas fa-times-circle text-red-400 mt-1"></i>
                            <span>No strong hook in first 3 seconds - 60% audience dropoff</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fas fa-times-circle text-red-400 mt-1"></i>
                            <span>Niche not clear - mixing tech reviews with vlogs confuses algorithm</span>
                        </li>
                    </ul>
                </div>

                <!-- Demo 7-Day Plan -->
                <div class="bg-gray-800/50 rounded-2xl p-6 border border-gray-700">
                    <h4 class="text-lg font-bold text-purple-400 mb-4 flex items-center gap-2">
                        <i class="fas fa-calendar-week"></i>
                        7-Day Fix Plan Preview
                    </h4>
                    <div class="space-y-3">
                        <div class="day-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-full bg-purple-500/20 flex items-center justify-center font-bold text-purple-400 border border-purple-500/30">1</div>
                            <div class="flex-1">
                                <h5 class="font-semibold text-sm">Improve Channel Banner & Bio</h5>
                                <p class="text-xs text-gray-400">Add value proposition and upload schedule</p>
                            </div>
                        </div>
                        <div class="day-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-full bg-purple-500/20 flex items-center justify-center font-bold text-purple-400 border border-purple-500/30">2</div>
                            <div class="flex-1">
                                <h5 class="font-semibold text-sm">Post 1 Short-Form Video</h5>
                                <p class="text-xs text-gray-400">Create 60s vertical video to increase reach</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="text-center pt-4 pb-2">
                    <button onclick="closeDemoReport(); scrollToTop();" class="btn-primary px-8 py-3 rounded-full font-bold text-lg w-full sm:w-auto">
                        Get Your Free Report Now
                    </button>
                    <p class="text-xs text-gray-500 mt-3">Takes 30 seconds • No signup required</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Email Capture Modal -->
    <div id="emailModal" class="hidden fixed inset-0 bg-black/95 z-50 flex items-center justify-center p-4 backdrop-blur-sm">
        <div class="glass-dark rounded-3xl max-w-md w-full p-8 modal-enter text-center border border-gray-700 shadow-2xl">
            <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-pink-500 rounded-full flex items-center justify-center mx-auto mb-4 shadow-lg shadow-purple-500/30">
                <i class="fas fa-envelope text-2xl"></i>
            </div>
            <h3 class="text-2xl font-bold mb-2">Almost Done! 🎉</h3>
            <p class="text-gray-400 mb-6">Enter your email to unlock your full diagnosis report and receive your personalized 7-day action plan via email.</p>
            
            <div class="space-y-4">
                <input 
                    type="email" 
                    id="userEmail" 
                    placeholder="your@email.com"
                    class="w-full px-4 py-3 bg-gray-800 border border-gray-700 rounded-xl text-white placeholder-gray-500 focus:outline-none focus:border-purple-500 focus:ring-2 focus:ring-purple-500/20 transition"
                    aria-label="Email address"
                >
                <button onclick="submitEmailAndShowResults()" class="w-full btn-primary py-3 rounded-xl font-bold text-lg">
                    Unlock Full Report
                </button>
                <button onclick="skipEmailAndShowResults()" class="text-gray-500 text-sm hover:text-gray-300 underline decoration-dotted">
                    Skip for now (Limited preview only)
                </button>
            </div>
            
            <div class="mt-6 pt-6 border-t border-gray-800">
                <div class="flex items-center justify-center gap-4 text-xs text-gray-600">
                    <span class="flex items-center gap-1"><i class="fas fa-lock"></i> Secure</span>
                    <span class="flex items-center gap-1"><i class="fas fa-user-shield"></i> No Spam</span>
                    <span class="flex items-center gap-1"><i class="fas fa-times-circle"></i> Unsubscribe Anytime</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Loading Section -->
    <section id="loadingSection" class="hidden fixed inset-0 bg-gray-900/98 z-50 flex items-center justify-center">
        <div class="text-center max-w-2xl px-4 w-full">
            <div class="relative w-24 h-24 md:w-32 md:h-32 mx-auto mb-8">
                <div class="absolute inset-0 border-4 border-purple-500/30 rounded-full"></div>
                <div class="absolute inset-0 border-4 border-purple-500 rounded-full border-t-transparent animate-spin"></div>
                <div class="absolute inset-4 bg-gradient-to-br from-purple-500 to-pink-500 rounded-full flex items-center justify-center shadow-lg shadow-purple-500/30">
                    <i class="fas fa-search text-2xl md:text-3xl text-white"></i>
                </div>
            </div>
            
            <h2 class="text-2xl md:text-3xl font-bold mb-6 brand-font">Analyzing Your Channel...</h2>
            <div class="space-y-3 text-left max-w-md mx-auto mb-6">
                <div class="flex items-center gap-3 text-gray-400 transition-all duration-300" id="step1">
                    <i class="fas fa-circle-notch fa-spin text-purple-400"></i>
                    <span>Scanning channel metadata...</span>
                </div>
                <div class="flex items-center gap-3 text-gray-400 transition-all duration-300" id="step2">
                    <i class="fas fa-circle text-xs text-gray-600"></i>
                    <span>Analyzing content strategy...</span>
                </div>
                <div class="flex items-center gap-3 text-gray-400 transition-all duration-300" id="step3">
                    <i class="fas fa-circle text-xs text-gray-600"></i>
                    <span>Checking engagement patterns...</span>
                </div>
                <div class="flex items-center gap-3 text-gray-400 transition-all duration-300" id="step4">
                    <i class="fas fa-circle text-xs text-gray-600"></i>
                    <span>Identifying growth blockers...</span>
                </div>
            </div>
            
            <div class="w-full max-w-md mx-auto bg-gray-800 rounded-full h-2 overflow-hidden border border-gray-700">
                <div class="h-full bg-gradient-to-r from-purple-500 to-pink-500 progress-fill shadow-[0_0_10px_rgba(168,85,247,0.5)]" id="progressBar" style="width: 0%"></div>
            </div>
            <p class="mt-4 text-purple-400 font-mono font-bold" id="progressText">0%</p>
            
            <p class="mt-6 text-sm text-gray-500 max-w-md mx-auto">
                <i class="fas fa-info-circle mr-1"></i>
                This may take up to 30 seconds for channels with many videos
            </p>
        </div>
    </section>

    <!-- Results Section -->
    <section id="resultsSection" class="hidden py-16 md:py-20 bg-gray-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <!-- Header -->
            <div class="text-center mb-12">
                <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-red-500/20 border border-red-500/30 text-red-400 mb-4 animate-pulse">
                    <i class="fas fa-exclamation-triangle"></i>
                    <span id="issueCount">12 Critical Issues Found</span>
                </div>
                <h2 class="text-3xl md:text-4xl font-bold mb-4 brand-font">Your Channel Diagnosis Report</h2>
                <p class="text-gray-400 max-w-2xl mx-auto">Here's exactly what's holding your channel back and how to fix it</p>
            </div>

            <!-- Overall Score with Breakdown -->
            <div class="glass-dark rounded-3xl p-6 md:p-8 mb-12 max-w-5xl mx-auto border border-gray-700 shadow-2xl">
                <div class="flex flex-col lg:flex-row items-center gap-8">
                    <!-- Main Score -->
                    <div class="relative flex-shrink-0">
                        <svg class="w-36 h-36 md:w-48 md:h-48 transform -rotate-90">
                            <circle cx="72" cy="72" r="64" stroke="#374151" stroke-width="12" fill="none"/>
                            <circle id="scoreCircle" cx="72" cy="72" r="64" stroke="#ef4444" stroke-width="12" fill="none" 
                                stroke-dasharray="402" stroke-dashoffset="402" stroke-linecap="round" class="score-ring"/>
                        </svg>
                        <div class="absolute inset-0 flex items-center justify-center flex-col">
                            <span class="text-4xl md:text-5xl font-bold" id="scoreValue">0</span>
                            <span class="text-xs md:text-sm text-gray-500 mt-1">Channel Score</span>
                            <span class="text-xs text-gray-600 mt-1">0-100</span>
                        </div>
                        <!-- Platform Badge -->
                        <div id="platformBadge" class="absolute -bottom-2 left-1/2 transform -translate-x-1/2 px-3 py-1 rounded-full bg-gray-800 border border-gray-700 text-xs font-semibold flex items-center gap-2">
                            <i class="fab fa-youtube text-red-500"></i>
                            <span>YouTube</span>
                        </div>
                    </div>
                    
                    <!-- Score Breakdown -->
                    <div class="flex-1 w-full">
                        <div class="mb-6 text-center lg:text-left">
                            <h3 class="text-xl md:text-2xl font-bold mb-2" id="scoreTitle">Needs Immediate Attention</h3>
                            <p class="text-gray-400 text-sm md:text-base" id="scoreDescription">Your channel has significant issues preventing growth. Follow the fixes below to improve.</p>
                        </div>

                        <!-- Detailed Scores -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 mb-6">
                            <div class="bg-gray-800/50 rounded-xl p-4 border border-gray-700 hover:border-purple-500/30 transition">
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-sm text-gray-400 flex items-center gap-2">
                                        <i class="fas fa-video text-purple-400"></i> Content Quality
                                    </span>
                                    <span class="font-bold" id="contentScore">72/100</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2 overflow-hidden">
                                    <div id="contentScoreBar" class="bg-yellow-400 h-2 rounded-full transition-all duration-1000" style="width: 0%"></div>
                                </div>
                            </div>
                            <div class="bg-gray-800/50 rounded-xl p-4 border border-gray-700 hover:border-purple-500/30 transition">
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-sm text-gray-400 flex items-center gap-2">
                                        <i class="fas fa-calendar-check text-pink-400"></i> Consistency
                                    </span>
                                    <span class="font-bold" id="consistencyScore">40/100</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2 overflow-hidden">
                                    <div id="consistencyScoreBar" class="bg-red-400 h-2 rounded-full transition-all duration-1000" style="width: 0%"></div>
                                </div>
                            </div>
                            <div class="bg-gray-800/50 rounded-xl p-4 border border-gray-700 hover:border-purple-500/30 transition">
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-sm text-gray-400 flex items-center gap-2">
                                        <i class="fas fa-image text-blue-400"></i> Thumbnail Power
                                    </span>
                                    <span class="font-bold" id="thumbnailScore">55/100</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2 overflow-hidden">
                                    <div id="thumbnailScoreBar" class="bg-yellow-400 h-2 rounded-full transition-all duration-1000" style="width: 0%"></div>
                                </div>
                            </div>
                            <div class="bg-gray-800/50 rounded-xl p-4 border border-gray-700 hover:border-purple-500/30 transition">
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-sm text-gray-400 flex items-center gap-2">
                                        <i class="fas fa-bolt text-yellow-400"></i> Hook Strength
                                    </span>
                                    <span class="font-bold" id="hookScore">60/100</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2 overflow-hidden">
                                    <div id="hookScoreBar" class="bg-yellow-400 h-2 rounded-full transition-all duration-1000" style="width: 0%"></div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="flex flex-wrap gap-3 justify-center lg:justify-start">
                            <span class="px-3 py-1.5 rounded-full bg-red-500/20 text-red-400 text-sm border border-red-500/30 font-medium">
                                <i class="fas fa-fire mr-1"></i> <span id="criticalCount">5</span> Critical
                            </span>
                            <span class="px-3 py-1.5 rounded-full bg-yellow-500/20 text-yellow-400 text-sm border border-yellow-500/30 font-medium">
                                <i class="fas fa-exclamation mr-1"></i> <span id="warningCount">4</span> Warnings
                            </span>
                            <span class="px-3 py-1.5 rounded-full bg-blue-500/20 text-blue-400 text-sm border border-blue-500/30 font-medium">
                                <i class="fas fa-info mr-1"></i> <span id="infoCount">3</span> Suggestions
                            </span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Detected Problems Section -->
            <div class="max-w-4xl mx-auto mb-12">
                <div class="bg-red-500/10 border border-red-500/30 rounded-2xl p-6 md:p-8">
                    <h3 class="text-xl md:text-2xl font-bold text-red-400 mb-6 flex items-center gap-3">
                        <i class="fas fa-bug"></i>
                        Critical Issues Detected
                    </h3>
                    <div id="detectedProblemsList" class="space-y-4">
                        <!-- Populated by JS -->
                    </div>
                </div>
            </div>

            <!-- Issues Grid -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6 mb-12" id="issuesContainer">
                <!-- Issues populated by JavaScript -->
            </div>

            <!-- 7-Day Action Plan Section -->
            <div class="glass-dark rounded-3xl p-6 md:p-8 max-w-5xl mx-auto mb-12 border border-gray-700">
                <h3 class="text-xl md:text-2xl font-bold mb-4 flex items-center gap-3">
                    <i class="fas fa-rocket text-purple-400"></i>
                    Your 7-Day Fix Plan
                </h3>
                <p class="text-gray-400 mb-6">Follow this day-by-day plan to fix your critical issues and boost your channel growth. Each task takes 15-30 minutes.</p>
                
                <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-4" id="sevenDayPlan">
                    <!-- Populated by JS -->
                </div>
            </div>

            <!-- Personalized Action Plan -->
            <div class="glass-dark rounded-3xl p-6 md:p-8 max-w-4xl mx-auto border border-gray-700">
                <h3 class="text-xl md:text-2xl font-bold mb-6 flex items-center gap-3">
                    <i class="fas fa-clipboard-check text-purple-400"></i>
                    Immediate Action Items
                </h3>
                <div class="space-y-4" id="actionPlan">
                    <!-- Action items populated by JavaScript -->
                </div>
            </div>

            <!-- Re-analyze Button -->
            <div class="text-center mt-12">
                <button onclick="resetAnalysis()" class="btn-primary px-8 py-4 rounded-full font-bold text-lg inline-flex items-center gap-2">
                    <i class="fas fa-redo"></i>
                    Analyze Another Channel
                </button>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="py-20 bg-gray-800/30 border-y border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4 brand-font">Trusted by 50,000+ Creators</h2>
                <p class="text-gray-400">See how ChannelDoctor helped creators fix their growth</p>
            </div>

            <div class="grid md:grid-cols-3 gap-6">
                <!-- Testimonial 1 -->
                <div class="testimonial-card rounded-2xl p-6">
                    <div class="flex items-center gap-1 mb-4 text-yellow-400 text-sm">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-300 mb-6 text-sm leading-relaxed">"I was stuck at 5K subs for months. ChannelDoctor found my thumbnail contrast issues and weak hooks. Fixed them and hit 10K in 3 weeks!"</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-blue-500 to-purple-500 flex items-center justify-center font-bold text-sm">MK</div>
                        <div>
                            <div class="font-semibold text-sm">Mike K.</div>
                            <div class="text-xs text-gray-500">@GamingWithMike • 45K subs</div>
                        </div>
                    </div>
                </div>

                <!-- Testimonial 2 -->
                <div class="testimonial-card rounded-2xl p-6">
                    <div class="flex items-center gap-1 mb-4 text-yellow-400 text-sm">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-300 mb-6 text-sm leading-relaxed">"The 7-day plan is genius. Instead of overwhelming me with 20 things to fix, it gave me one task per day. My TikTok views went from 200 to 5K average."</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-pink-500 to-red-500 flex items-center justify-center font-bold text-sm">SL</div>
                        <div>
                            <div class="font-semibold text-sm">Sarah L.</div>
                            <div class="text-xs text-gray-500">@FitnessWithSarah • 120K followers</div>
                        </div>
                    </div>
                </div>

                <!-- Testimonial 3 -->
                <div class="testimonial-card rounded-2xl p-6">
                    <div class="flex items-center gap-1 mb-4 text-yellow-400 text-sm">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-300 mb-6 text-sm leading-relaxed">"Best free tool I've used. The AI actually gives specific advice, not generic tips. Found out my upload schedule was killing my reach."</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-br from-green-500 to-blue-500 flex items-center justify-center font-bold text-sm">DJ</div>
                        <div>
                            <div class="font-semibold text-sm">David J.</div>
                            <div class="text-xs text-gray-500">@TechReviewsDaily • 80K subs</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Platform Logos -->
            <div class="mt-12 pt-12 border-t border-gray-800">
                <p class="text-center text-sm text-gray-500 mb-6">Works seamlessly with</p>
                <div class="flex justify-center items-center gap-8 md:gap-12 opacity-60 grayscale hover:grayscale-0 transition-all duration-500">
                    <div class="flex items-center gap-2 text-2xl md:text-3xl">
                        <i class="fab fa-youtube text-red-500"></i>
                        <span class="text-sm font-semibold hidden md:inline">YouTube</span>
                    </div>
                    <div class="flex items-center gap-2 text-2xl md:text-3xl">
                        <i class="fab fa-tiktok text-cyan-400"></i>
                        <span class="text-sm font-semibold hidden md:inline">TikTok</span>
                    </div>
                    <div class="flex items-center gap-2 text-2xl md:text-3xl opacity-50">
                        <i class="fab fa-instagram text-pink-500"></i>
                        <span class="text-sm font-semibold hidden md:inline">Coming Soon</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4 brand-font">Why ChannelDoctor is Different</h2>
                <p class="text-gray-400 max-w-2xl mx-auto">Unlike other tools that just show numbers, we tell you exactly what's wrong and how to fix it.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-red-500 to-orange-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-red-500/20">
                        <i class="fas fa-microscope text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Deep Channel Scan</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">We analyze everything from your bio to your latest post, identifying hidden mistakes that algorithms hate.</p>
                </div>

                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-purple-500 to-pink-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-purple-500/20">
                        <i class="fas fa-wrench text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Actionable Fixes</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Get step-by-step instructions with examples. No vague advice—just specific changes to make right now.</p>
                </div>

                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-blue-500 to-cyan-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-blue-500/20">
                        <i class="fas fa-chart-line text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Growth Prediction</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">See your potential growth if you fix the issues. We calculate exactly how many followers you could gain.</p>
                </div>

                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-green-500 to-emerald-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-green-500/20">
                        <i class="fas fa-robot text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">AI-Powered Analysis</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Our algorithm learns from thousands of successful channels to give you proven strategies that work.</p>
                </div>

                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-yellow-500 to-orange-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-yellow-500/20">
                        <i class="fas fa-bolt text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Instant Results</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">No waiting, no email required. Get your full diagnosis in under 30 seconds, completely free.</p>
                </div>

                <div class="glass-dark rounded-2xl p-8 hover-card border border-gray-800">
                    <div class="w-14 h-14 bg-gradient-to-br from-indigo-500 to-purple-500 rounded-xl flex items-center justify-center mb-6 shadow-lg shadow-indigo-500/20">
                        <i class="fas fa-shield-alt text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Privacy First</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">We don't store your data or require login. Analyze anonymously with complete privacy protection.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works -->
    <section id="how-it-works" class="py-20 bg-gray-800/30 border-y border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4 brand-font">How It Works</h2>
                <p class="text-gray-400">Three simple steps to transform your channel</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8 relative">
                <!-- Connecting Line (Desktop) -->
                <div class="hidden md:block absolute top-1/2 left-0 w-full h-1 bg-gradient-to-r from-purple-500 via-pink-500 to-red-500 transform -translate-y-1/2 z-0 opacity-30"></div>

                <div class="relative z-10 text-center">
                    <div class="w-16 h-16 md:w-20 md:h-20 bg-gradient-to-br from-purple-600 to-purple-800 rounded-full flex items-center justify-center mx-auto mb-6 text-xl md:text-2xl font-bold border-4 border-gray-900 shadow-lg shadow-purple-500/30">1</div>
                    <h3 class="text-lg md:text-xl font-bold mb-3">Paste Your URL</h3>
                    <p class="text-gray-400 text-sm">Enter any YouTube or TikTok channel link. Our AI immediately begins scanning.</p>
                </div>

                <div class="relative z-10 text-center">
                    <div class="w-16 h-16 md:w-20 md:h-20 bg-gradient-to-br from-pink-600 to-pink-800 rounded-full flex items-center justify-center mx-auto mb-6 text-xl md:text-2xl font-bold border-4 border-gray-900 shadow-lg shadow-pink-500/30">2</div>
                    <h3 class="text-lg md:text-xl font-bold mb-3">AI Diagnosis</h3>
                    <p class="text-gray-400 text-sm">Our system detects critical issues, scores your channel, and creates a 7-day fix plan.</p>
                </div>

                <div class="relative z-10 text-center">
                    <div class="w-16 h-16 md:w-20 md:h-20 bg-gradient-to-br from-red-600 to-red-800 rounded-full flex items-center justify-center mx-auto mb-6 text-xl md:text-2xl font-bold border-4 border-gray-900 shadow-lg shadow-red-500/30">3</div>
                    <h3 class="text-lg md:text-xl font-bold mb-3">Get Your Fix</h3>
                    <p class="text-gray-400 text-sm">Receive a detailed report with specific mistakes and step-by-step instructions to correct them.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="py-20 relative overflow-hidden">
        <div class="absolute inset-0 gradient-bg opacity-20"></div>
        <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
            <h2 class="text-3xl md:text-5xl font-bold mb-6 brand-font">Ready to Fix Your Channel?</h2>
            <p class="text-lg md:text-xl text-gray-300 mb-8">Join 50,000+ creators who transformed their social media presence with ChannelDoctor.</p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
                <button onclick="scrollToTop()" class="btn-primary px-10 py-4 rounded-full font-bold text-lg w-full sm:w-auto">
                    Get Free Audit Now
                </button>
                <button onclick="showDemoReport()" class="px-10 py-4 rounded-full font-bold text-lg border-2 border-white/20 hover:bg-white/10 transition w-full sm:w-auto">
                    View Example Report
                </button>
            </div>
            <p class="mt-6 text-sm text-gray-400 flex flex-wrap justify-center gap-4">
                <span class="flex items-center gap-1"><i class="fas fa-check text-green-400"></i> No credit card</span>
                <span class="flex items-center gap-1"><i class="fas fa-check text-green-400"></i> No signup required</span>
                <span class="flex items-center gap-1"><i class="fas fa-check text-green-400"></i> 100% Free</span>
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-4 gap-8 mb-8">
                <div>
                    <div class="flex items-center gap-2 mb-4">
                        <div class="w-8 h-8 bg-gradient-to-br from-purple-500 to-pink-500 rounded-lg flex items-center justify-center">
                            <i class="fas fa-stethoscope text-white text-sm"></i>
                        </div>
                        <span class="brand-font text-xl font-bold">ChannelDoctor</span>
                    </div>
                    <p class="text-gray-400 text-sm mb-4 leading-relaxed">The most advanced free channel analyzer on the internet. Fix your mistakes, grow your audience.</p>
                    <div class="flex gap-3">
                        <a href="#" class="w-8 h-8 rounded-full bg-gray-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gray-700 transition" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="w-8 h-8 rounded-full bg-gray-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gray-700 transition" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="w-8 h-8 rounded-full bg-gray-800 flex items-center justify-center text-gray-400 hover:text-white hover:bg-gray-700 transition" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-sm uppercase tracking-wider text-gray-300">Product</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li><a href="#features" class="hover:text-white transition">Features</a></li>
                        <li><a href="#how-it-works" class="hover:text-white transition">How It Works</a></li>
                        <li><a href="#" onclick="showDemoReport(); return false;" class="hover:text-white transition">Example Report</a></li>
                        <li><a href="#" class="hover:text-white transition">API Access</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-sm uppercase tracking-wider text-gray-300">Company</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li><a href="#" class="hover:text-white transition">About Us</a></li>
                        <li><a href="#" class="hover:text-white transition">Blog</a></li>
                        <li><a href="mailto:hello@channeldoctor.pro" class="hover:text-white transition">Contact</a></li>
                        <li><a href="#" class="hover:text-white transition">Partners</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4 text-sm uppercase tracking-wider text-gray-300">Legal</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li><a href="#" class="hover:text-white transition">Privacy Policy</a></li>
                        <li><a href="#" class="hover:text-white transition">Terms of Service</a></li>
                        <li><a href="#" class="hover:text-white transition">Cookie Policy</a></li>
                        <li><a href="#" class="hover:text-white transition">GDPR</a></li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-800 pt-8 flex flex-col md:flex-row justify-between items-center gap-4">
                <p class="text-gray-500 text-sm">© 2026 ChannelDoctor. All rights reserved.</p>
                <div class="flex items-center gap-6 text-sm text-gray-600">
                    <span class="flex items-center gap-2"><i class="fas fa-shield-alt text-green-500"></i> Privacy Protected</span>
                    <span class="flex items-center gap-2"><i class="fas fa-lock text-blue-500"></i> SSL Secured</span>
                </div>
            </div>
        </div>
    </footer>

    <!-- Feedback Widget -->
    <div class="feedback-btn rounded-full px-4 py-3 text-sm font-medium text-gray-300 hover:text-white transition shadow-lg hidden md:flex items-center gap-2 cursor-pointer" onclick="showFeedback()">
        <i class="fas fa-comment-dots"></i>
        <span>Feedback</span>
    </div>

    <!-- Feedback Modal -->
    <div id="feedbackModal" class="hidden fixed inset-0 bg-black/80 z-50 flex items-center justify-center p-4 backdrop-blur-sm">
        <div class="glass-dark rounded-2xl max-w-sm w-full p-6 modal-enter border border-gray-700">
            <h3 class="text-lg font-bold mb-4">Was this helpful?</h3>
            <div class="flex gap-3 mb-4">
                <button onclick="submitFeedback(true)" class="flex-1 py-3 rounded-xl bg-green-500/20 text-green-400 border border-green-500/30 hover:bg-green-500/30 transition flex items-center justify-center gap-2">
                    <i class="fas fa-thumbs-up"></i> Yes
                </button>
                <button onclick="submitFeedback(false)" class="flex-1 py-3 rounded-xl bg-red-500/20 text-red-400 border border-red-500/30 hover:bg-red-500/30 transition flex items-center justify-center gap-2">
                    <i class="fas fa-thumbs-down"></i> No
                </button>
            </div>
            <button onclick="closeFeedback()" class="w-full text-gray-500 text-sm hover:text-gray-300">Close</button>
        </div>
    </div>

    <script>
        // Global variables
        let currentIssues = [];
        let currentScore = 0;
        let currentPlatform = 'generic';
        let userEmailCollected = false;
        let analysisData = null;

        // Mobile Menu Toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        // Fill Example URL
        function fillExample(platform) {
            const examples = {
                youtube: 'https://youtube.com/c/mkbhd',
                tiktok: 'https://tiktok.com/@charlidamelio',
                instagram: 'https://instagram.com/natgeo'
            };
            document.getElementById('channelUrl').value = examples[platform];
            document.getElementById('channelUrl').focus();
            
            // Visual feedback
            const btn = event.currentTarget;
            btn.classList.add('scale-110');
            setTimeout(() => btn.classList.remove('scale-110'), 200);
        }

        // Demo Report Modal
        function showDemoReport() {
            document.getElementById('demoModal').classList.remove('hidden');
            document.body.style.overflow = 'hidden';
            gtag('event', 'view_demo_report');
        }

        function closeDemoReport() {
            document.getElementById('demoModal').classList.add('hidden');
            document.body.style.overflow = '';
        }

        // Close modal on outside click
        document.getElementById('demoModal').addEventListener('click', function(e) {
            if (e.target === this) closeDemoReport();
        });

        // Email Modal Functions
        function showEmailModal() {
            document.getElementById('emailModal').classList.remove('hidden');
            gtag('event', 'show_email_capture');
        }

        function closeEmailModal() {
            document.getElementById('emailModal').classList.add('hidden');
        }

        function submitEmailAndShowResults() {
            const email = document.getElementById('userEmail').value;
            if (!email || !email.includes('@')) {
                alert('Please enter a valid email address');
                return;
            }
            
            // Email validation regex
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(email)) {
                alert('Please enter a valid email address');
                return;
            }
            
            userEmailCollected = true;
            gtag('event', 'email_submitted', { 'platform': currentPlatform });
            closeEmailModal();
            displayResults(currentIssues, currentScore, currentPlatform);
            
            // Here you would typically send to your backend
            console.log('Email collected:', email);
        }

        function skipEmailAndShowResults() {
            userEmailCollected = false;
            gtag('event', 'email_skipped');
            closeEmailModal();
            displayResults(currentIssues.slice(0, 3), currentScore, currentPlatform, true);
        }

        // Enhanced Issues Database with Real YouTube API Integration Ready
        const issuesDatabase = {
            youtube: [
                {
                    severity: 'critical',
                    icon: 'fa-image',
                    title: 'Thumbnails Lack Contrast',
                    problem: 'Your thumbnails blend into the background. 70% of views come from browse features, and users scroll past low-contrast images.',
                    specificProblem: 'Low thumbnail contrast causing 60% scroll-past rate',
                    solution: 'Use high contrast colors (yellow/black, red/white). Add faces with emotions. Keep text under 3 words. Use Canva\'s "YouTube Thumbnail" templates.',
                    impact: 'High',
                    dayPlan: 'Improve thumbnail contrast using yellow/black colors',
                    metric: 'CTR below 2%'
                },
                {
                    severity: 'critical',
                    icon: 'fa-heading',
                    title: 'Weak Video Titles',
                    problem: 'You\'re describing the video instead of creating curiosity. Titles like "My Morning Routine" don\'t trigger clicks.',
                    specificProblem: 'Titles too descriptive, no curiosity gap',
                    solution: 'Use curiosity gaps: "I Tried [Celebrity]\'s Morning Routine... (Shocking Results)". Include brackets: [What Happened], [Storytime]. Use numbers when possible.',
                    impact: 'High',
                    dayPlan: 'Rewrite last 5 video titles with curiosity gaps',
                    metric: 'Average CTR 1.2%'
                },
                {
                    severity: 'critical',
                    icon: 'fa-video',
                    title: 'Slow First 30 Seconds',
                    problem: 'You lose 50% of viewers in the first 30 seconds because your intros are too long or unfocused.',
                    specificProblem: 'No strong hook in first 3 seconds',
                    solution: 'Start with the most exciting clip (b-roll). Use pattern interrupts every 5-10 seconds. Never start with "Hey guys, welcome back..."',
                    impact: 'Critical',
                    dayPlan: 'Add pattern interrupt in first 3 seconds of next video',
                    metric: '50% audience retention drop'
                },
                {
                    severity: 'warning',
                    icon: 'fa-calendar',
                    title: 'Inconsistent Upload Schedule',
                    problem: 'You uploaded 3 videos last month, then nothing for 3 weeks. Algorithms favor predictable patterns.',
                    specificProblem: 'Upload frequency too low (1-2 videos/month)',
                    solution: 'Pick a realistic schedule (even if 1x/week) and stick to it. Use YouTube Studio to schedule posts in advance. Consistency > Frequency.',
                    impact: 'Medium',
                    dayPlan: 'Set consistent upload schedule (minimum 1x/week)',
                    metric: '3 week gap detected'
                },
                {
                    severity: 'warning',
                    icon: 'fa-tags',
                    title: 'Missing SEO Optimization',
                    problem: 'Your video descriptions are under 100 words and lack keywords. You\'re missing searchable traffic.',
                    specificProblem: 'Descriptions under 100 words, missing keywords',
                    solution: 'Write 200+ word descriptions with timestamps. Research keywords using TubeBuddy or VidIQ. Include 3-5 relevant hashtags.',
                    impact: 'Medium',
                    dayPlan: 'Update last 3 video descriptions with 200+ words',
                    metric: 'SEO score: 23/100'
                },
                {
                    severity: 'info',
                    icon: 'fa-comments',
                    title: 'Low Community Engagement',
                    problem: 'You rarely reply to comments in the first hour. Early engagement signals quality to the algorithm.',
                    specificProblem: 'Not replying to comments in first hour',
                    solution: 'Pin a question in the first 10 minutes. Reply to 10+ comments within 1 hour of posting. Use heart reactions liberally.',
                    impact: 'Medium',
                    dayPlan: 'Reply to 20 comments within 1 hour of next upload',
                    metric: '0 replies in first hour'
                }
            ],
            tiktok: [
                {
                    severity: 'critical',
                    icon: 'fa-bolt',
                    title: 'Weak Hook in First 3 Seconds',
                    problem: 'You lose 60% of viewers in the first 3 seconds. Your hooks are too slow or unclear.',
                    specificProblem: '60% dropoff in first 3 seconds',
                    solution: 'Start with text overlay stating the outcome. Use pattern interrupts (zoom, sound effects). Never start with "Hey guys" or "So today..."',
                    impact: 'High',
                    dayPlan: 'Create 3 hooks with text overlay in first frame',
                    metric: '3s view rate: 40%'
                },
                {
                    severity: 'critical',
                    icon: 'fa-music',
                    title: 'Not Using Trending Audio',
                    problem: 'Original audio gets 40% less reach than trending sounds. You\'re fighting the algorithm.',
                    specificProblem: 'Using original audio instead of trending sounds',
                    solution: 'Check TikTok Creative Center weekly for trending sounds. Use sounds with <100K videos for better chances of viral.',
                    impact: 'High',
                    dayPlan: 'Find and use 3 trending sounds this week',
                    metric: '0 trending sounds used'
                },
                {
                    severity: 'warning',
                    icon: 'fa-closed-captioning',
                    title: 'Captions Too Small',
                    problem: 'Users watch TikTok on mute in public. Your captions are hard to read or missing.',
                    specificProblem: 'Captions too small or missing',
                    solution: 'Use large, high-contrast captions (yellow text with black outline). Keep on-screen text under 5 words per frame.',
                    impact: 'High',
                    dayPlan: 'Add large captions to next 5 videos',
                    metric: 'Caption readability: Poor'
                }
            ],
            generic: [
                {
                    severity: 'critical',
                    icon: 'fa-bullseye',
                    title: 'No Clear Niche',
                    problem: 'You post about cooking, then fitness, then travel. Algorithms can\'t categorize your content.',
                    specificProblem: 'Niche not clear - mixing unrelated topics',
                    solution: 'Pick 1 main niche and 2 sub-niches. Stick to them for 90 days. Example: Fitness > Home Workouts > Busy Professionals.',
                    impact: 'Critical',
                    dayPlan: 'Define your 1 main niche and 2 sub-niches',
                    metric: '5 different topics in last 10 posts'
                },
                {
                    severity: 'critical',
                    icon: 'fa-hand-point-up',
                    title: 'Missing Call-to-Action',
                    problem: 'You never ask viewers to follow, like, or comment. You\'re leaving engagement on the table.',
                    specificProblem: 'No CTA in videos or bio',
                    solution: 'End every post with: "Follow for part 2" or "Comment YES if you agree" or "Save this for later".',
                    impact: 'High',
                    dayPlan: 'Add strong CTA to bio and next 3 posts',
                    metric: '0 CTAs found'
                },
                {
                    severity: 'warning',
                    icon: 'fa-chart-bar',
                    title: 'Ignoring Analytics',
                    problem: 'You\'re creating content blindly without looking at what actually performs.',
                    specificProblem: 'Not checking analytics weekly',
                    solution: 'Check analytics weekly. Double down on top 20% performing content. Cut bottom 20% content types.',
                    impact: 'Medium',
                    dayPlan: 'Review analytics and identify top 3 performing videos',
                    metric: 'Last checked: Never'
                }
            ]
        };

        // 7-Day Action Plan Templates
        const dayPlans = [
            { day: 1, action: 'Audit & fix channel banner/bio', icon: 'fa-id-card', time: '20 min' },
            { day: 2, action: 'Create 1 short-form video', icon: 'fa-video', time: '30 min' },
            { day: 3, action: 'Fix thumbnail contrast', icon: 'fa-image', time: '25 min' },
            { day: 4, action: 'Add strong hooks to content', icon: 'fa-bolt', time: '20 min' },
            { day: 5, action: 'Engage with 20 comments', icon: 'fa-comments', time: '15 min' },
            { day: 6, action: 'Research trending topics', icon: 'fa-search', time: '20 min' },
            { day: 7, action: 'Plan next week\'s content', icon: 'fa-calendar', time: '30 min' }
        ];

        function detectPlatform(url) {
            if (!url) return 'generic';
            const lowerUrl = url.toLowerCase();
            if (lowerUrl.includes('youtube.com') || lowerUrl.includes('youtu.be')) return 'youtube';
            if (lowerUrl.includes('tiktok.com')) return 'tiktok';
            if (lowerUrl.includes('instagram.com')) return 'instagram';
            return 'generic';
        }

        function generateIssues(platform) {
            let issues = [];
            
            if (issuesDatabase[platform]) {
                issues = [...issuesDatabase[platform]];
            }
            
            // Add generic issues
            const randomGeneric = issuesDatabase.generic.sort(() => 0.5 - Math.random()).slice(0, 2);
            issues = [...issues, ...randomGeneric];
            
            // Shuffle and limit to 6
            return issues.sort(() => 0.5 - Math.random()).slice(0, 6);
        }

        function calculateDetailedScores(issues) {
            let contentScore = 70 + Math.floor(Math.random() * 20);
            let consistencyScore = 40 + Math.floor(Math.random() * 30);
            let thumbnailScore = 50 + Math.floor(Math.random() * 25);
            let hookScore = 45 + Math.floor(Math.random() * 30);
            
            // Adjust based on issues
            issues.forEach(issue => {
                if (issue.title.includes('Thumbnail')) thumbnailScore -= 15;
                if (issue.title.includes('Title') || issue.title.includes('Content')) contentScore -= 10;
                if (issue.title.includes('Schedule') || issue.title.includes('Consistency')) consistencyScore -= 20;
                if (issue.title.includes('Hook')) hookScore -= 15;
            });
            
            return {
                content: Math.max(0, Math.min(100, contentScore)),
                consistency: Math.max(0, Math.min(100, consistencyScore)),
                thumbnail: Math.max(0, Math.min(100, thumbnailScore)),
                hook: Math.max(0, Math.min(100, hookScore))
            };
        }

        function calculateScore(issues) {
            let score = 100;
            issues.forEach(issue => {
                if (issue.severity === 'critical') score -= 12;
                else if (issue.severity === 'warning') score -= 6;
                else score -= 3;
            });
            return Math.max(15, score);
        }

        // Simulated API Call (Replace with real YouTube Data API)
        async function fetchChannelData(url, platform) {
            // This is where you'd integrate YouTube Data API v3
            // Example: const response = await fetch(`https://www.googleapis.com/youtube/v3/channels?part=snippet,statistics&id=${channelId}&key=${API_KEY}`);
            
            // For demo, we simulate API delay and return mock data
            await new Promise(resolve => setTimeout(resolve, 1500));
            
            return {
                platform: platform,
                subscribers: Math.floor(Math.random() * 50000) + 1000,
                videos: Math.floor(Math.random() * 200) + 10,
                views: Math.floor(Math.random() * 1000000),
                joined: '2020-' + (Math.floor(Math.random() * 12) + 1),
                isRealData: false // Flag to indicate this is simulated
            };
        }

        async function startAnalysis() {
            const url = document.getElementById('channelUrl').value.trim();
            
            if (!url) {
                alert('Please enter a valid URL');
                return;
            }

            if (!url.includes('http')) {
                alert('Please enter a valid URL starting with http:// or https://');
                return;
            }

            // Track event
            gtag('event', 'start_analysis', { 'platform': detectPlatform(url) });

            // Show loading
            document.getElementById('loadingSection').classList.remove('hidden');
            
            currentPlatform = detectPlatform(url);
            
            // Simulate API fetch
            try {
                analysisData = await fetchChannelData(url, currentPlatform);
            } catch (error) {
                console.error('API Error:', error);
            }
            
            // Simulate progress steps
            const steps = ['step1', 'step2', 'step3', 'step4'];
            const progressBar = document.getElementById('progressBar');
            const progressText = document.getElementById('progressText');
            
            for (let i = 0; i < steps.length; i++) {
                await new Promise(r => setTimeout(r, 800));
                
                // Update completed step
                const stepEl = document.getElementById(steps[i]);
                stepEl.innerHTML = '<i class="fas fa-check-circle text-green-400"></i><span class="text-green-400">' + stepEl.querySelector('span').textContent + '</span>';
                
                // Update next step
                if (i < steps.length - 1) {
                    const nextEl = document.getElementById(steps[i + 1]);
                    nextEl.innerHTML = '<i class="fas fa-circle-notch fa-spin text-purple-400"></i><span>' + nextEl.querySelector('span').textContent + '</span>';
                }
                
                const progress = ((i + 1) / steps.length) * 100;
                progressBar.style.width = progress + '%';
                progressText.textContent = Math.round(progress) + '%';
            }
            
            await new Promise(r => setTimeout(r, 500));
            
            // Generate results
            currentIssues = generateIssues(currentPlatform);
            currentScore = calculateScore(currentIssues);
            
            // Hide loading
            document.getElementById('loadingSection').classList.add('hidden');
            
            // Reset steps for next time
            setTimeout(() => {
                const stepTexts = [
                    'Scanning channel metadata...',
                    'Analyzing content strategy...',
                    'Checking engagement patterns...',
                    'Identifying growth blockers...'
                ];
                steps.forEach((step, index) => {
                    document.getElementById(step).innerHTML = `<i class="fas fa-circle text-xs text-gray-600"></i><span>${stepTexts[index]}</span>`;
                });
                document.getElementById('step1').innerHTML = '<i class="fas fa-circle-notch fa-spin text-purple-400"></i><span>Scanning channel metadata...</span>';
                progressBar.style.width = '0%';
            }, 500);
            
            // Show email capture modal
            showEmailModal();
        }

        function getScoreColor(score) {
            if (score >= 80) return 'text-green-400';
            if (score >= 60) return 'text-yellow-400';
            return 'text-red-400';
        }

        function getScoreBarColor(score) {
            if (score >= 80) return 'bg-green-400';
            if (score >= 60) return 'bg-yellow-400';
            return 'bg-red-400';
        }

        function displayResults(issues, score, platform, isLimited = false) {
            // Update platform badge
            const platformBadge = document.getElementById('platformBadge');
            if (platform === 'youtube') {
                platformBadge.innerHTML = '<i class="fab fa-youtube text-red-500"></i><span>YouTube</span>';
            } else if (platform === 'tiktok') {
                platformBadge.innerHTML = '<i class="fab fa-tiktok text-cyan-400"></i><span>TikTok</span>';
            } else {
                platformBadge.innerHTML = '<i class="fas fa-globe text-gray-400"></i><span>Generic</span>';
            }

            // Update score circle
            const scoreCircle = document.getElementById('scoreCircle');
            const circumference = 402; // 2 * PI * 64
            const offset = circumference - (score / 100) * circumference;
            
            setTimeout(() => {
                scoreCircle.style.strokeDashoffset = offset;
                
                if (score >= 80) {
                    scoreCircle.style.stroke = '#10b981';
                    document.getElementById('scoreTitle').textContent = 'Excellent Condition';
                    document.getElementById('scoreTitle').className = 'text-xl md:text-2xl font-bold mb-2 text-green-400';
                    document.getElementById('scoreDescription').textContent = 'Your channel is in great shape! Minor tweaks will take you to the next level. Estimated growth: +15% monthly.';
                } else if (score >= 60) {
                    scoreCircle.style.stroke = '#f59e0b';
                    document.getElementById('scoreTitle').textContent = 'Needs Improvement';
                    document.getElementById('scoreTitle').className = 'text-xl md:text-2xl font-bold mb-2 text-yellow-400';
                    document.getElementById('scoreDescription').textContent = 'Good foundation, but several issues are limiting your growth potential. Fix these to unlock faster growth.';
                } else {
                    scoreCircle.style.stroke = '#ef4444';
                    document.getElementById('scoreTitle').textContent = 'Critical Issues Found';
                    document.getElementById('scoreTitle').className = 'text-xl md:text-2xl font-bold mb-2 text-red-400';
                    document.getElementById('scoreDescription').textContent = 'Your channel has significant problems preventing growth. Immediate action recommended to avoid further decline.';
                }
            }, 100);

            // Animate score number
            let currentScoreNum = 0;
            const scoreInterval = setInterval(() => {
                if (currentScoreNum >= score) {
                    clearInterval(scoreInterval);
                } else {
                    currentScoreNum++;
                    document.getElementById('scoreValue').textContent = currentScoreNum;
                }
            }, 20);

            // Update detailed scores with animation
            const detailedScores = calculateDetailedScores(issues);
            
            setTimeout(() => {
                document.getElementById('contentScore').textContent = detailedScores.content + '/100';
                document.getElementById('contentScore').className = 'font-bold ' + getScoreColor(detailedScores.content);
                document.getElementById('contentScoreBar').style.width = detailedScores.content + '%';
                document.getElementById('contentScoreBar').className = 'h-2 rounded-full transition-all duration-1000 ' + getScoreBarColor(detailedScores.content);
                
                document.getElementById('consistencyScore').textContent = detailedScores.consistency + '/100';
                document.getElementById('consistencyScore').className = 'font-bold ' + getScoreColor(detailedScores.consistency);
                document.getElementById('consistencyScoreBar').style.width = detailedScores.consistency + '%';
                document.getElementById('consistencyScoreBar').className = 'h-2 rounded-full transition-all duration-1000 ' + getScoreBarColor(detailedScores.consistency);
                
                document.getElementById('thumbnailScore').textContent = detailedScores.thumbnail + '/100';
                document.getElementById('thumbnailScore').className = 'font-bold ' + getScoreColor(detailedScores.thumbnail);
                document.getElementById('thumbnailScoreBar').style.width = detailedScores.thumbnail + '%';
                document.getElementById('thumbnailScoreBar').className = 'h-2 rounded-full transition-all duration-1000 ' + getScoreBarColor(detailedScores.thumbnail);
                
                document.getElementById('hookScore').textContent = detailedScores.hook + '/100';
                document.getElementById('hookScore').className = 'font-bold ' + getScoreColor(detailedScores.hook);
                document.getElementById('hookScoreBar').style.width = detailedScores.hook + '%';
                document.getElementById('hookScoreBar').className = 'h-2 rounded-full transition-all duration-1000 ' + getScoreBarColor(detailedScores.hook);
            }, 500);

            // Update issue counts
            const criticalCount = issues.filter(i => i.severity === 'critical').length;
            const warningCount = issues.filter(i => i.severity === 'warning').length;
            const infoCount = issues.filter(i => i.severity === 'info').length;
            
            document.getElementById('issueCount').textContent = `${issues.length} Issues Found (${criticalCount} Critical)`;
            document.getElementById('criticalCount').textContent = criticalCount;
            document.getElementById('warningCount').textContent = warningCount;
            document.getElementById('infoCount').textContent = infoCount;

            // Populate Detected Problems List
            const problemsList = document.getElementById('detectedProblemsList');
            problemsList.innerHTML = '';
            issues.filter(i => i.severity === 'critical').slice(0, 4).forEach(issue => {
                const div = document.createElement('div');
                div.className = 'flex items-start gap-3 bg-gray-800/50 rounded-lg p-4 border border-red-500/20 hover:border-red-500/40 transition';
                div.innerHTML = `
                    <i class="fas fa-times-circle text-red-400 mt-0.5 flex-shrink-0"></i>
                    <div>
                        <span class="text-gray-300 text-sm font-medium block">${issue.specificProblem || issue.problem.substring(0, 60) + '...'}</span>
                        ${issue.metric ? `<span class="text-xs text-red-400/80 mt-1 block"><i class="fas fa-chart-line mr-1"></i>${issue.metric}</span>` : ''}
                    </div>
                `;
                problemsList.appendChild(div);
            });

            // Display issues cards
            const container = document.getElementById('issuesContainer');
            container.innerHTML = '';
            
            if (isLimited) {
                // Show limited preview message
                const limitedMsg = document.createElement('div');
                limitedMsg.className = 'col-span-full glass-dark rounded-2xl p-8 text-center border-2 border-dashed border-purple-500/30';
                limitedMsg.innerHTML = `
                    <div class="w-16 h-16 bg-purple-500/20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-lock text-2xl text-purple-400"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-2">Full Report Locked</h3>
                    <p class="text-gray-400 mb-4 max-w-md mx-auto">Enter your email to unlock all ${currentIssues.length} issues and your complete 7-day fix plan with detailed guides.</p>
                    <button onclick="showEmailModal()" class="btn-primary px-6 py-3 rounded-full font-semibold">
                        Unlock Full Report
                    </button>
                `;
                container.appendChild(limitedMsg);
            }
            
            issues.forEach((issue, index) => {
                const severityColors = {
                    critical: 'red',
                    warning: 'yellow',
                    info: 'blue'
                };
                
                const color = severityColors[issue.severity];
                
                const card = document.createElement('div');
                card.className = `glass-dark rounded-2xl p-6 hover-card severity-${issue.severity} opacity-0 transform translate-y-4 transition-all duration-500 border border-gray-800 hover:border-${color}-500/30`;
                card.style.animationDelay = `${index * 100}ms`;
                
                card.innerHTML = `
                    <div class="flex items-start justify-between mb-4">
                        <div class="w-12 h-12 bg-${color}-500/20 rounded-xl flex items-center justify-center border border-${color}-500/30">
                            <i class="fas ${issue.icon} text-${color}-400 text-xl"></i>
                        </div>
                        <span class="px-3 py-1 rounded-full bg-${color}-500/20 text-${color}-400 text-xs font-bold uppercase border border-${color}-500/30">
                            ${issue.severity}
                        </span>
                    </div>
                    <h3 class="text-lg font-bold mb-2">${issue.title}</h3>
                    <p class="text-gray-400 text-sm mb-4 leading-relaxed">${issue.problem}</p>
                    <div class="bg-gray-800/50 rounded-xl p-4 border border-gray-700">
                        <div class="flex items-center gap-2 mb-2 text-green-400 text-sm font-bold">
                            <i class="fas fa-check-circle"></i>
                            <span>How to Fix</span>
                        </div>
                        <p class="text-gray-300 text-sm leading-relaxed">${issue.solution}</p>
                    </div>
                    <div class="mt-4 flex items-center justify-between text-xs">
                        <span class="text-gray-500 flex items-center gap-1">
                            <i class="fas fa-chart-line"></i>
                            Impact: ${issue.impact}
                        </span>
                        ${issue.metric ? `<span class="text-${color}-400 font-medium">${issue.metric}</span>` : ''}
                    </div>
                `;
                
                container.appendChild(card);
                
                // Animate in
                setTimeout(() => {
                    card.classList.remove('opacity-0', 'translate-y-4');
                }, index * 100);
            });

            // Generate 7-Day Plan
            const sevenDayContainer = document.getElementById('sevenDayPlan');
            sevenDayContainer.innerHTML = '';
            
            // Use issue-specific day plans if available
            const criticalIssues = issues.filter(i => i.severity === 'critical');
            
            dayPlans.forEach((day, index) => {
                // Override with specific issue plan if available
                if (criticalIssues[index] && criticalIssues[index].dayPlan) {
                    day.action = criticalIssues[index].dayPlan;
                }
                
                const dayCard = document.createElement('div');
                dayCard.className = 'day-card rounded-xl p-4 flex flex-col items-center text-center gap-3 cursor-pointer';
                dayCard.innerHTML = `
                    <div class="w-10 h-10 rounded-full bg-purple-500/20 flex items-center justify-center font-bold text-purple-400 border border-purple-500/30 text-sm">
                        ${day.day}
                    </div>
                    <div class="flex-1">
                        <h5 class="font-semibold text-sm mb-1 leading-tight">${day.action}</h5>
                        <span class="text-xs text-gray-500"><i class="far fa-clock mr-1"></i>${day.time}</span>
                    </div>
                    <i class="fas ${day.icon} text-gray-500 text-sm"></i>
                `;
                
                // Add click to mark complete (visual only)
                dayCard.addEventListener('click', function() {
                    this.classList.toggle('completed');
                    const icon = this.querySelector('.fa-check');
                    if (this.classList.contains('completed')) {
                        if (!icon) {
                            const check = document.createElement('i');
                            check.className = 'fas fa-check text-green-400 absolute top-2 right-2 text-xs';
                            this.appendChild(check);
                        }
                    }
                });
                
                sevenDayContainer.appendChild(dayCard);
            });

            // Generate Action Plan
            const actionPlan = document.getElementById('actionPlan');
            actionPlan.innerHTML = '';
            
            const topIssues = issues.filter(i => i.severity === 'critical').slice(0, 3);
            if (topIssues.length === 0) topIssues.push(issues[0]);
            
            topIssues.forEach((issue, index) => {
                const item = document.createElement('div');
                item.className = 'flex items-start gap-4 p-4 rounded-xl bg-gray-800/30 border border-gray-700 hover:border-purple-500/50 transition group cursor-pointer';
                item.innerHTML = `
                    <div class="w-8 h-8 rounded-full bg-purple-500/20 flex items-center justify-center flex-shrink-0 border border-purple-500/30 group-hover:bg-purple-500/30 transition">
                        <span class="text-purple-400 font-bold text-sm">${index + 1}</span>
                    </div>
                    <div class="flex-1">
                        <h4 class="font-semibold mb-1 group-hover:text-purple-400 transition">${issue.title}</h4>
                        <p class="text-sm text-gray-400 mb-2 line-clamp-2">${issue.solution}</p>
                        <button class="text-purple-400 text-xs hover:text-purple-300 transition flex items-center gap-1 font-medium" onclick="alert('Detailed guide coming soon! This would open a step-by-step tutorial.')">
                            <span>View detailed guide</span>
                            <i class="fas fa-arrow-right text-xs"></i>
                        </button>
                    </div>
                `;
                actionPlan.appendChild(item);
            });
            
            // Add priority tip
            const tip = document.createElement('div');
            tip.className = 'mt-6 p-4 rounded-xl bg-gradient-to-r from-purple-500/20 to-pink-500/20 border border-purple-500/30';
            tip.innerHTML = `
                <div class="flex items-start gap-3">
                    <i class="fas fa-lightbulb text-yellow-400 text-xl mt-1"></i>
                    <div>
                        <h4 class="font-semibold mb-1 text-purple-300">Pro Tip</h4>
                        <p class="text-sm text-gray-300 leading-relaxed">Focus on fixing the Critical issues first. They have 3x more impact on your growth than minor optimizations. Start with "${topIssues[0].title}" today.</p>
                    </div>
                </div>
            `;
            actionPlan.appendChild(tip);

            // Show results section
            document.getElementById('resultsSection').classList.remove('hidden');
            document.getElementById('resultsSection').scrollIntoView({ behavior: 'smooth', block: 'start' });
            
            // Track view
            gtag('event', 'view_results', { 
                'platform': platform,
                'score': score,
                'email_collected': userEmailCollected
            });
        }

        function resetAnalysis() {
            document.getElementById('resultsSection').classList.add('hidden');
            document.getElementById('channelUrl').value = '';
            document.getElementById('progressBar').style.width = '0%';
            document.getElementById('progressText').textContent = '0%';
            
            // Reset score circle
            document.getElementById('scoreCircle').style.strokeDashoffset = 402;
            
            window.scrollTo({ top: 0, behavior: 'smooth' });
            document.getElementById('channelUrl').focus();
            
            gtag('event', 'reset_analysis');
        }

        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
            document.getElementById('channelUrl').focus();
        }

        // Enter key support
        document.getElementById('channelUrl').addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                startAnalysis();
            }
        });

        // Feedback functions
        function showFeedback() {
            document.getElementById('feedbackModal').classList.remove('hidden');
        }

        function closeFeedback() {
            document.getElementById('feedbackModal').classList.add('hidden');
        }

        function submitFeedback(wasHelpful) {
            gtag('event', 'feedback', { 'helpful': wasHelpful });
            closeFeedback();
            
            // Show thank you toast
            const toast = document.createElement('div');
            toast.className = 'fixed bottom-4 left-1/2 transform -translate-x-1/2 bg-green-500 text-white px-6 py-3 rounded-full shadow-lg z-50 animate-bounce';
            toast.innerHTML = '<i class="fas fa-check-circle mr-2"></i>Thank you for your feedback!';
            document.body.appendChild(toast);
            setTimeout(() => toast.remove(), 3000);
        }

        // Close modals on escape key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeDemoReport();
                closeEmailModal();
                closeFeedback();
            }
        });

        // Initialize
        document.addEventListener('DOMContentLoaded', function() {
            // Check for URL parameters (for tracking)
            const urlParams = new URLSearchParams(window.location.search);
            const ref = urlParams.get('ref');
            if (ref) {
                gtag('event', 'page_view', { 'ref': ref });
            }
        });
    </script>
</body>
</html>
