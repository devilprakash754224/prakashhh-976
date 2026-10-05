<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ZYVORA AVAITION  | Redefining Luxury Private Aviation</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Playfair Display & Montserrat -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        obsidian: '#0A0B0E',
                        'obsidian-card': '#12141A',
                        'obsidian-light': '#1A1D26',
                        gold: {
                            100: '#FAF3E0',
                            300: '#E5C07B',
                            400: '#D4AF37',
                            500: '#C59B27',
                            600: '#9A7718',
                        },
                        champagne: '#F4E8C1',
                        'champagne-dark': '#B8A375'
                    },
                    fontFamily: {
                        serif: ['"Playfair Display"', 'serif'],
                        sans: ['"Montserrat"', 'sans-serif'],
                    },
                    backgroundImage: {
                        'gold-gradient': 'linear-gradient(135deg, #F4E8C1 0%, #D4AF37 50%, #9A7718 100%)',
                        'dark-gradient': 'linear-gradient(180deg, rgba(10, 11, 14, 0.6) 0%, rgba(10, 11, 14, 0.95) 100%)',
                        'radial-glow': 'radial-gradient(circle at center, rgba(212, 175, 55, 0.15) 0%, rgba(10, 11, 14, 0) 70%)',
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom Luxury Scrollbars and Gold Metallic Accents */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #0A0B0E;
        }
        ::-webkit-scrollbar-thumb {
            background: #332a15;
            border-radius: 3px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #D4AF37;
        }
        .text-gold-gradient {
            background: linear-gradient(135deg, #FFF5D6 0%, #D4AF37 50%, #AA820A 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .border-gold-gradient {
            border-image: linear-gradient(to right, #D4AF37, #B8A375, #5E4B1A) 1;
        }
        .gold-glow {
            box-shadow: 0 0 25px rgba(212, 175, 55, 0.2);
        }
        .gold-glow-hover:hover {
            box-shadow: 0 0 35px rgba(212, 175, 55, 0.35);
            border-color: rgba(212, 175, 55, 0.8);
        }
        .glass-panel {
            background: rgba(18, 20, 26, 0.75);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(212, 175, 55, 0.18);
        }
        .glass-panel-gold {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.08) 0%, rgba(18, 20, 26, 0.85) 100%);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(212, 175, 55, 0.3);
        }
    </style>
</head>
<body class="bg-obsidian text-gray-200 font-sans selection:bg-gold-400 selection:text-obsidian overflow-x-hidden">

    <!-- NAVIGATION BAR -->
    <header id="navbar" class="fixed top-0 left-0 w-full z-50 transition-all duration-500 py-6 px-6 md:px-12 glass-panel border-b border-white/5">
        <div class="max-w-7xl mx-auto flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-10 h-10 rounded-full border border-gold-400/50 flex items-center justify-center transition-all duration-500 group-hover:rotate-45 group-hover:border-gold-400">
                    <i class="fa-solid fa-plane-up text-gold-400 text-lg"></i>
                </div>
                <div class="flex flex-col">
                    <span class="font-serif text-2xl font-bold tracking-widest text-gold-gradient uppercase">ZYVORA2.O</span>
                    <span class="text-[9px] uppercase tracking-[0.35em] text-gray-400 -mt-1">Private Aviation</span>
                </div>
            </a>

            <!-- Desktop Nav Links -->
            <nav class="hidden lg:flex items-center space-x-10 text-xs tracking-[0.25em] uppercase font-medium text-gray-300">
                <a href="#about" class="hover:text-gold-400 transition-colors duration-300">Overview</a>
                <a href="#fleet" class="hover:text-gold-400 transition-colors duration-300">The Fleet</a>
                <a href="#services" class="hover:text-gold-400 transition-colors duration-300">Bespoke Services</a>
                <a href="#experience" class="hover:text-gold-400 transition-colors duration-300">In-Flight Customizer</a>
                <a href="#membership" class="hover:text-gold-400 transition-colors duration-300">Jet Card</a>
            </nav>

            <!-- Actions -->
            <div class="hidden md:flex items-center space-x-6">
                <a href="#inquiry" class="text-xs uppercase tracking-widest text-gold-300 hover:text-white transition-colors duration-300 flex items-center gap-2">
                    <i class="fa-solid fa-phone-volume text-gold-400"></i> +916372193827
                </a>
                <button onclick="toggleModal('charterModal')" class="px-6 py-2.5 rounded-full text-xs font-semibold uppercase tracking-widest bg-gold-gradient text-obsidian shadow-lg hover:brightness-110 transition-all duration-300 transform hover:-translate-y-0.5">
                    Request Quote
                </button>
            </div>

            <!-- Mobile Hamburger Button -->
            <button id="mobileMenuBtn" class="lg:hidden text-gold-400 text-2xl focus:outline-none">
                <i class="fa-solid fa-bars"></i>
            </button>
        </div>

        <!-- Mobile Menu Drawer -->
        <div id="mobileMenu" class="hidden lg:hidden fixed inset-x-0 top-[80px] bg-obsidian-card border-b border-gold-400/20 p-6 shadow-2xl flex flex-col space-y-4 text-center">
            <a href="#about" class="mobile-link text-sm uppercase tracking-widest text-gray-300 hover:text-gold-400 py-2">Overview</a>
            <a href="#fleet" class="mobile-link text-sm uppercase tracking-widest text-gray-300 hover:text-gold-400 py-2">The Fleet</a>
            <a href="#services" class="mobile-link text-sm uppercase tracking-widest text-gray-300 hover:text-gold-400 py-2">Bespoke Services</a>
            <a href="#experience" class="mobile-link text-sm uppercase tracking-widest text-gray-300 hover:text-gold-400 py-2">In-Flight Customizer</a>
            <a href="#membership" class="mobile-link text-sm uppercase tracking-widest text-gray-300 hover:text-gold-400 py-2">Jet Card</a>
            <button onclick="toggleModal('charterModal'); toggleMobileMenu();" class="w-full py-3 text-xs font-semibold uppercase tracking-widest bg-gold-gradient text-obsidian rounded-full mt-4">
                Request Quote
            </button>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative min-h-screen flex items-center justify-center pt-28 pb-20 px-4 sm:px-6 lg:px-8 overflow-hidden">
        <!-- Background Imagery & Cinematic FX -->
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?auto=format&fit=crop&w=2000&q=80" 
                 alt="Private Luxury Jet Wing Above Clouds" 
                 class="w-full h-full object-cover object-center opacity-40 scale-105 animate-pulse" 
                 style="animation-duration: 12s;"
                 onerror="this.src='https://placehold.co/1920x1080/0A0B0E/D4AF37?text=Aureus+Luxury+Jets'">
            <div class="absolute inset-0 bg-gradient-to-t from-obsidian via-obsidian/70 to-obsidian/40"></div>
            <div class="absolute inset-0 bg-radial-glow"></div>
        </div>

        <div class="relative z-10 max-w-7xl mx-auto w-full text-center flex flex-col items-center">
            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full border border-gold-400/30 bg-gold-400/10 mb-6 backdrop-blur-md">
                <span class="w-2 h-2 rounded-full bg-gold-400 animate-ping"></span>
                <span class="text-xs font-medium uppercase tracking-[0.3em] text-champagne">The Pinnacle of Global Charter</span>
            </div>

            <h1 class="font-serif text-4xl sm:text-6xl md:text-7xl font-bold tracking-tight text-white max-w-4xl leading-tight">
                Elevate Your Journey Beyond <span class="text-gold-gradient italic font-normal">Boundaries</span>
            </h1>
            <p class="mt-6 text-base sm:text-lg text-gray-300 max-w-2xl font-light tracking-wide leading-relaxed">
                Unrivaled comfort, absolute privacy, and seamless hyper-luxury tailored to the exact specifications of the global elite.
            </p>

            <!-- FLIGHT SEARCH / BOOKING ENGINE WIDGET -->
            <div class="mt-10 w-full max-w-5xl glass-panel-gold rounded-3xl p-6 sm:p-8 shadow-2xl relative text-left">
                <div class="flex flex-wrap items-center justify-between gap-4 border-b border-gold-400/20 pb-4 mb-6">
                    <div class="flex items-center space-x-2 sm:space-x-4 text-xs font-semibold tracking-wider uppercase">
                        <button id="typeOneWay" onclick="setFlightType('oneWay')" class="px-4 py-2 rounded-full bg-gold-400 text-obsidian transition-all">One Way</button>
                        <button id="typeRoundTrip" onclick="setFlightType('roundTrip')" class="px-4 py-2 rounded-full text-gray-300 hover:text-gold-300 transition-all">Round Trip</button>
                        <button id="typeMultiLeg" onclick="setFlightType('multiLeg')" class="px-4 py-2 rounded-full text-gray-300 hover:text-gold-300 transition-all">Multi-City</button>
                    </div>
                    <div class="text-xs text-gold-300 flex items-center gap-2">
                        <i class="fa-solid fa-shield-halved"></i> Guaranteed 2-Hour Dispatch Rate
                    </div>
                </div>

                <form id="heroFlightForm" onsubmit="handleHeroSearch(event)" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-5 gap-4">
                    <!-- Origin -->
                    <div class="flex flex-col space-y-1.5">
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold">From</label>
                        <div class="relative">
                            <i class="fa-solid fa-plane-departure absolute left-3 top-1/2 -translate-y-1/2 text-gold-400/60 text-xs"></i>
                            <input type="text" required placeholder="New York (KTEB)" value="New York (KTEB)" class="w-full bg-obsidian/80 border border-gold-400/20 rounded-xl py-3 pl-9 pr-3 text-xs text-white focus:outline-none focus:border-gold-400 transition-all">
                        </div>
                    </div>

                    <!-- Destination -->
                    <div class="flex flex-col space-y-1.5">
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold">To</label>
                        <div class="relative">
                            <i class="fa-solid fa-plane-arrival absolute left-3 top-1/2 -translate-y-1/2 text-gold-400/60 text-xs"></i>
                            <input type="text" required placeholder="Geneva (LSGG)" value="Geneva (LSGG)" class="w-full bg-obsidian/80 border border-gold-400/20 rounded-xl py-3 pl-9 pr-3 text-xs text-white focus:outline-none focus:border-gold-400 transition-all">
                        </div>
                    </div>

                    <!-- Departure Date -->
                    <div class="flex flex-col space-y-1.5">
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold">Departure Date</label>
                        <div class="relative">
                            <i class="fa-regular fa-calendar-days absolute left-3 top-1/2 -translate-y-1/2 text-gold-400/60 text-xs"></i>
                            <input type="date" required value="2026-10-15" class="w-full bg-obsidian/80 border border-gold-400/20 rounded-xl py-3 pl-9 pr-3 text-xs text-white focus:outline-none focus:border-gold-400 transition-all">
                        </div>
                    </div>

                    <!-- Aircraft Preference -->
                    <div class="flex flex-col space-y-1.5">
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold">Aircraft Class</label>
                        <div class="relative">
                            <i class="fa-solid fa-crown absolute left-3 top-1/2 -translate-y-1/2 text-gold-400/60 text-xs"></i>
                            <select class="w-full bg-obsidian/80 border border-gold-400/20 rounded-xl py-3 pl-9 pr-3 text-xs text-white focus:outline-none focus:border-gold-400 transition-all appearance-none cursor-pointer">
                                <option value="ultra-long">Ultra Long Range (12-16 seats)</option>
                                <option value="heavy">Heavy Jet (10-14 seats)</option>
                                <option value="super-mid">Super Midsize (8-9 seats)</option>
                                <option value="v VIP">VIP Airliner (18+ seats)</option>
                            </select>
                        </div>
                    </div>

                    <!-- Search Button -->
                    <div class="flex items-end">
                        <button type="submit" class="w-full h-[42px] bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-xl hover:brightness-110 transition-all flex items-center justify-center gap-2 shadow-lg">
                            <span>Search Flight</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                    </div>
                </form>
            </div>
            
            <!-- Quick Metrics -->
            <div class="mt-16 grid grid-cols-2 md:grid-cols-4 gap-8 max-w-4xl w-full border-t border-gold-400/10 pt-8 text-center">
                <div>
                    <p class="font-serif text-3xl font-bold text-gold-gradient">7,500+</p>
                    <p class="text-xs text-gray-400 uppercase tracking-widest mt-1">Airports Worldwide</p>
                </div>
                <div>
                    <p class="font-serif text-3xl font-bold text-gold-gradient">99.8%</p>
                    <p class="text-xs text-gray-400 uppercase tracking-widest mt-1">On-Time Reliability</p>
                </div>
                <div>
                    <p class="font-serif text-3xl font-bold text-gold-gradient">150+</p>
                    <p class="text-xs text-gray-400 uppercase tracking-widest mt-1">Bespoke Aircraft</p>
                </div>
                <div>
                    <p class="font-serif text-3xl font-bold text-gold-gradient">24/7/365</p>
                    <p class="text-xs text-gray-400 uppercase tracking-widest mt-1">Personal Concierge</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FLEET SHOWCASE SECTION -->
    <section id="fleet" class="py-24 px-6 md:px-12 bg-obsidian-card relative overflow-hidden">
        <div class="max-w-7xl mx-auto">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 border-b border-gold-400/15 pb-6">
                <div>
                    <span class="text-xs uppercase tracking-[0.3em] text-gold-400 font-semibold">Flagship Jet Collection</span>
                    <h2 class="font-serif text-3xl md:text-5xl font-bold text-white mt-2">The Zyvora Fleet</h2>
                </div>
                <!-- Fleet Filter Tabs -->
                <div class="mt-6 md:mt-0 flex flex-wrap gap-2 text-xs font-semibold tracking-widest uppercase">
                    <button onclick="filterFleet('all')" class="fleet-tab active px-5 py-2.5 rounded-full border border-gold-400 bg-gold-400 text-obsidian transition-all">All Aircraft</button>
                    <button onclick="filterFleet('ultra-long')" class="fleet-tab px-5 py-2.5 rounded-full border border-gold-400/30 text-gray-400 hover:border-gold-400 transition-all">Ultra Long Range</button>
                    <button onclick="filterFleet('heavy')" class="fleet-tab px-5 py-2.5 rounded-full border border-gold-400/30 text-gray-400 hover:border-gold-400 transition-all">Heavy Jets</button>
                    <button onclick="filterFleet('executive')" class="fleet-tab px-5 py-2.5 rounded-full border border-gold-400/30 text-gray-400 hover:border-gold-400 transition-all">Executive</button>
                </div>
            </div>

            <!-- Fleet Grid -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8" id="fleetGrid">
                
                <!-- Jet Card 1 -->
                <div class="fleet-item ultra-long glass-panel rounded-3xl overflow-hidden group border border-gold-400/20 hover:border-gold-400/60 transition-all duration-500 flex flex-col justify-between">
                    <div>
                        <div class="relative h-64 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1583416750470-965b2707b355?auto=format&fit=crop&w=1000&q=80" 
                                 alt="Bombardier Global 7500" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700"
                                 onerror="this.src='https://placehold.co/800x600/12141A/D4AF37?text=Bombardier+Global+7500'">
                            <span class="absolute top-4 left-4 bg-obsidian/80 backdrop-blur-md text-gold-300 text-[10px] font-bold uppercase tracking-widest px-3 py-1 rounded-full border border-gold-400/30">Ultra Long Range</span>
                        </div>
                        <div class="p-6">
                            <h3 class="font-serif text-2xl font-bold text-white group-hover:text-gold-300 transition-colors">Bombardier Global 7500</h3>
                            <p class="text-xs text-gray-400 mt-2 font-light">The largest and longest-range business jet, featuring four true living spaces and a master suite.</p>
                            
                            <!-- Specs Grid -->
                            <div class="grid grid-cols-2 gap-4 mt-6 pt-6 border-t border-gold-400/10 text-xs">
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Range</span>
                                    <span class="text-gold-300 font-semibold text-sm">7,700 NM</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Speed</span>
                                    <span class="text-gold-300 font-semibold text-sm">Mach 0.925</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Passengers</span>
                                    <span class="text-gold-300 font-semibold text-sm">Up to 19</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Cabin Height</span>
                                    <span class="text-gold-300 font-semibold text-sm">6 ft 2 in</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <button onclick="openFleetModal('Bombardier Global 7500', '7,700 NM', 'Mach 0.925', '19 Passengers', 'Dedicated Master Suite, Ka-band High Speed WiFi, Nuage Ergonomic Seating, Private Stateroom with Shower.')" class="w-full py-3 rounded-xl border border-gold-400/30 text-gold-300 hover:bg-gold-gradient hover:text-obsidian hover:border-transparent font-semibold text-xs uppercase tracking-widest transition-all">
                            View Full Specifications
                        </button>
                    </div>
                </div>

                <!-- Jet Card 2 -->
                <div class="fleet-item ultra-long glass-panel rounded-3xl overflow-hidden group border border-gold-400/20 hover:border-gold-400/60 transition-all duration-500 flex flex-col justify-between">
                    <div>
                        <div class="relative h-64 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?auto=format&fit=crop&w=1000&q=80" 
                                 alt="Gulfstream G700" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700"
                                 onerror="this.src='https://placehold.co/800x600/12141A/D4AF37?text=Gulfstream+G700'">
                            <span class="absolute top-4 left-4 bg-obsidian/80 backdrop-blur-md text-gold-300 text-[10px] font-bold uppercase tracking-widest px-3 py-1 rounded-full border border-gold-400/30">Flagship Heavy</span>
                        </div>
                        <div class="p-6">
                            <h3 class="font-serif text-2xl font-bold text-white group-hover:text-gold-300 transition-colors">Gulfstream G700</h3>
                            <p class="text-xs text-gray-400 mt-2 font-light">An unprecedented cabin environment with 20 panoramic oval windows and whisper-quiet sound levels.</p>
                            
                            <!-- Specs Grid -->
                            <div class="grid grid-cols-2 gap-4 mt-6 pt-6 border-t border-gold-400/10 text-xs">
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Range</span>
                                    <span class="text-gold-300 font-semibold text-sm">7,500 NM</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Speed</span>
                                    <span class="text-gold-300 font-semibold text-sm">Mach 0.90</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Passengers</span>
                                    <span class="text-gold-300 font-semibold text-sm">Up to 15</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Cabin Height</span>
                                    <span class="text-gold-300 font-semibold text-sm">6 ft 3 in</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <button onclick="openFleetModal('Gulfstream G700', '7,500 NM', 'Mach 0.90', '15 Passengers', '100% Fresh Air Circulated Every 2 Mins, Circadian Lighting System, Ultra-Gallley with Wine Chiller.')" class="w-full py-3 rounded-xl border border-gold-400/30 text-gold-300 hover:bg-gold-gradient hover:text-obsidian hover:border-transparent font-semibold text-xs uppercase tracking-widest transition-all">
                            View Full Specifications
                        </button>
                    </div>
                </div>

                <!-- Jet Card 3 -->
                <div class="fleet-item heavy executive glass-panel rounded-3xl overflow-hidden group border border-gold-400/20 hover:border-gold-400/60 transition-all duration-500 flex flex-col justify-between">
                    <div>
                        <div class="relative h-64 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1520437358207-323b43b50729?auto=format&fit=crop&w=1000&q=80" 
                                 alt="Dassault Falcon 10X" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700"
                                 onerror="this.src='https://placehold.co/800x600/12141A/D4AF37?text=Dassault+Falcon+10X'">
                            <span class="absolute top-4 left-4 bg-obsidian/80 backdrop-blur-md text-gold-300 text-[10px] font-bold uppercase tracking-widest px-3 py-1 rounded-full border border-gold-400/30">Executive Jet</span>
                        </div>
                        <div class="p-6">
                            <h3 class="font-serif text-2xl font-bold text-white group-hover:text-gold-300 transition-colors">Dassault Falcon 10X</h3>
                            <p class="text-xs text-gray-400 mt-2 font-light">Modular luxury architecture crafted with French artisan elegance and advanced fighter-jet technology.</p>
                            
                            <!-- Specs Grid -->
                            <div class="grid grid-cols-2 gap-4 mt-6 pt-6 border-t border-gold-400/10 text-xs">
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Range</span>
                                    <span class="text-gold-300 font-semibold text-sm">7,500 NM</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Max Speed</span>
                                    <span class="text-gold-300 font-semibold text-sm">Mach 0.925</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Passengers</span>
                                    <span class="text-gold-300 font-semibold text-sm">Up to 16</span>
                                </div>
                                <div>
                                    <span class="text-gray-500 uppercase tracking-wider block text-[10px]">Cabin Height</span>
                                    <span class="text-gold-300 font-semibold text-sm">6 ft 8 in</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <button onclick="openFleetModal('Dassault Falcon 10X', '7,500 NM', 'Mach 0.925', '16 Passengers', 'Widest Cabin in Business Aviation, Queen-Size Bed Suite, HEPA Air Filtration, Military HUD Systems.')" class="w-full py-3 rounded-xl border border-gold-400/30 text-gold-300 hover:bg-gold-gradient hover:text-obsidian hover:border-transparent font-semibold text-xs uppercase tracking-widest transition-all">
                            View Full Specifications
                        </button>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section id="services" class="py-24 px-6 md:px-12 bg-obsidian relative">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-400 font-semibold">Unmatched Privilege</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold text-white mt-2">Bespoke Aviation Services</h2>
                <p class="text-gray-400 text-sm mt-4">Every detail curated to deliver an effortless, elevated travel ecosystem for royalty, corporate leaders, and discerning individuals.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-plane"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Private Jet Charter</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Instant access to over 7,500 airports worldwide with zero positioning fees for members. Complete confidentiality guaranteed.</p>
                </div>

                <!-- Service 2 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-bell-concierge"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Michelin In-Flight Dining</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Custom culinary itineraries paired with sommelier-selected rare vintages, prepared in flight by elite private chefs.</p>
                </div>

                <!-- Service 3 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-helicopter"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Helicopter Transfers</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Seamless door-to-tarmac transfers avoiding urban congestion with our private fleet of Sikorsky and Airbus helicopters.</p>
                </div>

                <!-- Service 4 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-briefcase"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Aircraft Management</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Comprehensive asset optimization, crew selection, regulatory compliance, and charter revenue offset for jet owners.</p>
                </div>

                <!-- Service 5 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-bolt"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Empty Leg Opportunities</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Exclusive access to repositioning flights at preferential charter rates with full luxury service standards.</p>
                </div>

                <!-- Service 6 -->
                <div class="glass-panel rounded-3xl p-8 hover:-translate-y-2 transition-all duration-500 group border border-gold-400/10 hover:border-gold-400/50">
                    <div class="w-14 h-14 rounded-2xl bg-gold-400/10 border border-gold-400/30 flex items-center justify-center text-gold-400 text-2xl mb-6 group-hover:bg-gold-gradient group-hover:text-obsidian transition-all">
                        <i class="fa-solid fa-shield-halved"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-white mb-3">Diplomatic & Executive Security</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">Discrete armed escort, secure vehicle convoys, and specialized protocol management anywhere across the globe.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- INTERACTIVE IN-FLIGHT CUSTOMIZER SECTION -->
    <section id="experience" class="py-24 px-6 md:px-12 bg-obsidian-card relative overflow-hidden border-y border-gold-400/10">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-400 font-semibold">Tailored Ambiance</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold text-white mt-2">Design Your Flight Experience</h2>
                <p class="text-gray-400 text-sm mt-4">Preview your high-altitude sanctuary by selecting lighting, gastronomy, and cabin configurations in real time.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center">
                <!-- Customizer Preview Screen -->
                <div class="lg:col-span-7 glass-panel-gold rounded-3xl p-6 sm:p-8 relative min-h-[420px] flex flex-col justify-between overflow-hidden shadow-2xl">
                    <div id="previewBackground" class="absolute inset-0 z-0 transition-all duration-700 bg-cover bg-center" 
                         style="background-image: url('https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?auto=format&fit=crop&w=1200&q=80');">
                        <div id="previewOverlay" class="absolute inset-0 bg-obsidian/60 transition-all duration-500"></div>
                    </div>

                    <!-- Live Customizer Status Badges -->
                    <div class="relative z-10 flex flex-wrap gap-2">
                        <span id="activeAmbianceTag" class="px-3 py-1 rounded-full bg-gold-400/90 text-obsidian font-bold text-[10px] uppercase tracking-widest">
                            Sunset Silk Ambiance
                        </span>
                        <span id="activeCateringTag" class="px-3 py-1 rounded-full bg-obsidian/80 text-champagne border border-gold-400/30 text-[10px] font-semibold uppercase tracking-widest">
                            Osetra Caviar & Dom Pérignon
                        </span>
                    </div>

                    <!-- Dynamic Quote Summary -->
                    <div class="relative z-10 bg-obsidian/90 backdrop-blur-md rounded-2xl p-6 border border-gold-400/30 mt-32">
                        <h4 class="font-serif text-xl font-bold text-gold-300" id="previewTitle">Executive Lounge Suite</h4>
                        <p class="text-xs text-gray-300 mt-1 font-light" id="previewDesc">Relaxing warm amber circadian lighting designed to minimize jet lag over long-haul oceanic flights.</p>
                        <div class="mt-4 flex items-center justify-between border-t border-gold-400/20 pt-4 text-xs">
                            <span class="text-gray-400">Atmosphere Score:</span>
                            <span class="text-gold-400 font-bold tracking-widest uppercase">100% Bespoke</span>
                        </div>
                    </div>
                </div>

                <!-- Customizer Controls -->
                <div class="lg:col-span-5 space-y-6">
                    
                    <!-- Control 1: Ambiance -->
                    <div class="glass-panel p-6 rounded-2xl border border-gold-400/20">
                        <label class="text-xs uppercase tracking-widest text-gold-300 font-semibold block mb-3">1. Select Cabin Ambiance</label>
                        <div class="grid grid-cols-3 gap-2 text-xs">
                            <button onclick="setCustomizerAmbiance('sunset')" class="ambiance-btn active p-3 rounded-xl border border-gold-400 bg-gold-400/20 text-white font-medium hover:border-gold-400 transition-all text-center">
                                Sunset Amber
                            </button>
                            <button onclick="setCustomizerAmbiance('midnight')" class="ambiance-btn p-3 rounded-xl border border-gold-400/20 text-gray-400 font-medium hover:border-gold-400 transition-all text-center">
                                Midnight Blue
                            </button>
                            <button onclick="setCustomizerAmbiance('zen')" class="ambiance-btn p-3 rounded-xl border border-gold-400/20 text-gray-400 font-medium hover:border-gold-400 transition-all text-center">
                                Zen Daylight
                            </button>
                        </div>
                    </div>

                    <!-- Control 2: Catering -->
                    <div class="glass-panel p-6 rounded-2xl border border-gold-400/20">
                        <label class="text-xs uppercase tracking-widest text-gold-300 font-semibold block mb-3">2. Culinary Selection</label>
                        <select id="cateringSelect" onchange="updateCustomizerCatering()" class="w-full bg-obsidian border border-gold-400/30 rounded-xl p-3 text-xs text-white focus:outline-none focus:border-gold-400">
                            <option value="caviar">Osetra Caviar & Vintage Champagne Pairing</option>
                            <option value="omakase">Private Chef High-Altitude Japanese Omakase</option>
                            <option value="mediterranean">Michelin-Star Mediterranean Degustation</option>
                            <option value="wellbeing">Organic Bio-Hacking & Longevity Menu</option>
                        </select>
                    </div>

                    <!-- Control 3: Entertainment & Amenities -->
                    <div class="glass-panel p-6 rounded-2xl border border-gold-400/20">
                        <label class="text-xs uppercase tracking-widest text-gold-300 font-semibold block mb-3">3. Suite Amenities</label>
                        <div class="space-y-2 text-xs text-gray-300">
                            <label class="flex items-center space-x-3 cursor-pointer">
                                <input type="checkbox" checked class="accent-gold-400 rounded">
                                <span>Starlink Low-Latency Ultra WiFi</span>
                            </label>
                            <label class="flex items-center space-x-3 cursor-pointer">
                                <input type="checkbox" checked class="accent-gold-400 rounded">
                                <span>Hermès Silk Sleep Kit & Amenities</span>
                            </label>
                            <label class="flex items-center space-x-3 cursor-pointer">
                                <input type="checkbox" class="accent-gold-400 rounded">
                                <span>Private High-Altitude Spa Massage Therapist</span>
                            </label>
                        </div>
                    </div>

                    <button onclick="toggleModal('charterModal')" class="w-full py-4 bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-2xl hover:brightness-110 transition-all shadow-xl">
                        Save Configuration & Book
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- JET CARD MEMBERSHIP TIERS -->
    <section id="membership" class="py-24 px-6 md:px-12 bg-obsidian relative">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-400 font-semibold">The Aureus Club</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold text-white mt-2">Jet Card Membership Tiers</h2>
                <p class="text-gray-400 text-sm mt-4">Fixed hourly rates, guaranteed jet availability with 12-hour notice, and zero peak-day surcharges.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Silver Tier -->
                <div class="glass-panel rounded-3xl p-8 flex flex-col justify-between border border-gold-400/20 hover:border-gold-400/50 transition-all">
                    <div>
                        <span class="text-xs uppercase tracking-widest text-gray-400 font-bold">Entry Privileges</span>
                        <h3 class="font-serif text-2xl font-bold text-white mt-1">Silver Jet Card</h3>
                        <p class="text-3xl font-serif font-bold text-gold-gradient mt-4">$150,000 <span class="text-xs font-sans text-gray-400 font-normal">/ deposit</span></p>

                        <ul class="mt-8 space-y-4 text-xs text-gray-300">
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Guaranteed 24-Hour Aircraft Dispatch
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Fixed Hourly Rates (Super-Midsize)
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Complimentary Catering Allowance
                            </li>
                            <li class="flex items-center gap-3 opacity-50">
                                <i class="fa-solid fa-xmark text-gray-600"></i> Helicopter Tarmac Transfers
                            </li>
                        </ul>
                    </div>
                    <button onclick="toggleModal('charterModal')" class="mt-8 w-full py-3 rounded-xl border border-gold-400/40 text-gold-300 font-semibold text-xs uppercase tracking-widest hover:bg-gold-400 hover:text-obsidian transition-all">
                        Select Silver
                    </button>
                </div>

                <!-- Gold Tier -->
                <div class="glass-panel-gold rounded-3xl p-8 flex flex-col justify-between border-2 border-gold-400 relative transform md:-translate-y-4 shadow-2xl">
                    <span class="absolute -top-3 left-1/2 -translate-x-1/2 bg-gold-gradient text-obsidian text-[10px] font-bold uppercase tracking-widest px-4 py-1 rounded-full">
                        Most Popular
                    </span>
                    <div>
                        <span class="text-xs uppercase tracking-widest text-gold-300 font-bold">Executive Tier</span>
                        <h3 class="font-serif text-2xl font-bold text-white mt-1">Gold Jet Card</h3>
                        <p class="text-3xl font-serif font-bold text-gold-gradient mt-4">$350,000 <span class="text-xs font-sans text-gray-400 font-normal">/ deposit</span></p>

                        <ul class="mt-8 space-y-4 text-xs text-gray-200">
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Guaranteed 12-Hour Aircraft Dispatch
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Access to Ultra Long Range Fleet
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Preferred Michelin Dining Menu
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> 2 Free Helicopter Transfers / Year
                            </li>
                        </ul>
                    </div>
                    <button onclick="toggleModal('charterModal')" class="mt-8 w-full py-3.5 rounded-xl bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest hover:brightness-110 transition-all shadow-lg">
                        Select Gold Member
                    </button>
                </div>

                <!-- Obsidian Signature -->
                <div class="glass-panel rounded-3xl p-8 flex flex-col justify-between border border-gold-400/20 hover:border-gold-400/50 transition-all">
                    <div>
                        <span class="text-xs uppercase tracking-widest text-gold-400 font-bold">By Invitation</span>
                        <h3 class="font-serif text-2xl font-bold text-white mt-1">Obsidian Signature</h3>
                        <p class="text-3xl font-serif font-bold text-gold-gradient mt-4">$750,000+ <span class="text-xs font-sans text-gray-400 font-normal">/ deposit</span></p>

                        <ul class="mt-8 space-y-4 text-xs text-gray-300">
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Guaranteed 6-Hour Dispatch Anywhere
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Dedicated Fleet Tail Lock
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Unlimited Helicopter Transfers
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fa-solid fa-check text-gold-400"></i> Dedicated Global Executive Concierge
                            </li>
                        </ul>
                    </div>
                    <button onclick="toggleModal('charterModal')" class="mt-8 w-full py-3 rounded-xl border border-gold-400/40 text-gold-300 font-semibold text-xs uppercase tracking-widest hover:bg-gold-400 hover:text-obsidian transition-all">
                        Apply for Obsidian
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- TESTIMONIALS SECTION -->
    <section class="py-24 px-6 md:px-12 bg-obsidian-card border-t border-gold-400/10">
        <div class="max-w-6xl mx-auto text-center">
            <i class="fa-solid fa-quote-left text-4xl text-gold-400/40 mb-6"></i>
            <h2 class="font-serif text-2xl sm:text-4xl italic text-gray-200 max-w-4xl mx-auto leading-relaxed">
                "Zyvora Jets has transformed our transatlantic travel. From the discrete tarmac transfers to the Michelin-standard dining at 45,000 feet, their commitment to perfection is absolute."
            </h2>
            <div class="mt-8">
                <p class="font-serif font-bold text-gold-gradient text-lg">Lord Jaganath swami Vance</p>
                <p class="text-xs uppercase tracking-widest text-gray-400">Managing Director, Vance Global Capital</p>
            </div>
        </div>
    </section>

    <!-- CONTACT / PRIVATE INQUIRY SECTION -->
    <section id="inquiry" class="py-24 px-6 md:px-12 bg-obsidian relative">
        <div class="max-w-4xl mx-auto glass-panel-gold rounded-3xl p-8 sm:p-12 border border-gold-400/30">
            <div class="text-center mb-10">
                <span class="text-xs uppercase tracking-[0.3em] text-gold-400 font-semibold">Discrete Consultation</span>
                <h2 class="font-serif text-3xl font-bold text-white mt-1">Private Flight Inquiry</h2>
                <p class="text-gray-400 text-xs mt-2">Connect directly with a Senior Aviation Advisor within 15 minutes.</p>
            </div>

            <form id="inquiryForm" onsubmit="handleInquirySubmit(event)" class="space-y-6">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <div>
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold block mb-1">Full Name</label>
                        <input type="text" required placeholder="Sir subham , sri prakash" class="w-full bg-obsidian/90 border border-gold-400/20 rounded-xl p-3.5 text-xs text-white focus:outline-none focus:border-gold-400">
                    </div>
                    <div>
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold block mb-1">Private Email</label>
                        <input type="email" required placeholder="zyvora@avaition.com" class="w-full bg-obsidian/90 border border-gold-400/20 rounded-xl p-3.5 text-xs text-white focus:outline-none focus:border-gold-400">
                    </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <div>
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold block mb-1">Direct Telephone</label>
                        <input type="tel" required placeholder="+1 (555) 019-2831" class="w-full bg-obsidian/90 border border-gold-400/20 rounded-xl p-3.5 text-xs text-white focus:outline-none focus:border-gold-400">
                    </div>
                    <div>
                        <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold block mb-1">Preferred Contact Method</label>
                        <select class="w-full bg-obsidian/90 border border-gold-400/20 rounded-xl p-3.5 text-xs text-white focus:outline-none focus:border-gold-400">
                            <option>Encrypted-whatsapp-6372193827</option>
                            <option>Direct Phone Call</option>
                            <option>Confidential Email</option>
                        </select>
                    </div>
                </div>

                <div>
                    <label class="text-[10px] uppercase tracking-widest text-gold-300 font-semibold block mb-1">Specific Requirements / Itinerary Details</label>
                    <textarea rows="4" placeholder="Detail your routing, passenger count, security protocol, or dietary requirements..." class="w-full bg-obsidian/90 border border-gold-400/20 rounded-xl p-3.5 text-xs text-white focus:outline-none focus:border-gold-400"></textarea>
                </div>

                <button type="submit" class="w-full py-4 bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-xl hover:brightness-110 transition-all shadow-xl">
                    Dispatch Private Advisor
                </button>
            </form>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-obsidian border-t border-gold-400/10 py-12 px-6 md:px-12 text-gray-400 text-xs">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6">
            <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-full border border-gold-400/50 flex items-center justify-center">
                    <i class="fa-solid fa-plane-up text-gold-400 text-xs"></i>
                </div>
                <span class="font-serif text-lg font-bold tracking-widest text-gold-gradient uppercase">Zyvora Jets</span>
            </div>
            <p class="text-center md:text-left text-gray-500">
                &copy; 2026 Zyvora Aviation Group Ltd. All rights reserved. Operating under FAA Part 135 & EASA Air Operator Certification.
            </p>
            <div class="flex space-x-6 text-gold-400/70 text-base">
                <a href="#" class="hover:text-gold-400"><i class="fa-brands fa-instagram"></i></a>
                <a href="#" class="hover:text-gold-400"><i class="fa-brands fa-linkedin-in"></i></a>
                <a href="#" class="hover:text-gold-400"><i class="fa-brands fa-twitter"></i></a>
                        <a href="#" class="hover:text-gold-400"><i class="fa-brands fa-reddit"></i></a>
            </div>
        </div>
    </footer>

    <!-- CHARTER / FLEET SPEC MODAL -->
    <div id="charterModal" class="fixed inset-0 z-50 bg-obsidian/90 backdrop-blur-xl flex items-center justify-center p-4 hidden">
        <div class="bg-obsidian-card border border-gold-400/40 rounded-3xl max-w-lg w-full p-8 relative shadow-2xl">
            <button onclick="toggleModal('charterModal')" class="absolute top-6 right-6 text-gray-400 hover:text-gold-400 text-xl">
                <i class="fa-solid fa-xmark"></i>
            </button>

            <h3 id="modalTitle" class="font-serif text-2xl font-bold text-white">Private Charter Quote</h3>
            <p id="modalSub" class="text-xs text-gold-300 mt-1">Direct Advisor Access & Instant Route Calculation</p>

            <div id="modalContent" class="mt-6 space-y-4 text-xs text-gray-300">
                <p class="leading-relaxed">Your tailored flight plan is being generated. Enter your phone number below for immediate SMS itinerary confirmation from our flight operations desk.</p>
                <input type="tel" placeholder="+1 (800) 000-0000" class="w-full bg-obsidian border border-gold-400/30 rounded-xl p-3 text-xs text-white">
                <button onclick="submitModalQuote()" class="w-full py-3 bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-xl hover:brightness-110">
                    Confirm Concierge Request
                </button>
            </div>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mobileMenu = document.getElementById('mobileMenu');
        
        mobileMenuBtn.addEventListener('click', toggleMobileMenu);

        function toggleMobileMenu() {
            mobileMenu.classList.toggle('hidden');
        }

        // Modal Handler
        function toggleModal(modalId) {
            const modal = document.getElementById(modalId);
            modal.classList.toggle('hidden');
        }

        // Fleet Filtering System
        function filterFleet(category) {
            const tabs = document.querySelectorAll('.fleet-tab');
            tabs.forEach(tab => {
                tab.classList.remove('bg-gold-400', 'text-obsidian');
                tab.classList.add('text-gray-400');
            });
            event.target.classList.add('bg-gold-400', 'text-obsidian');
            event.target.classList.remove('text-gray-400');

            const items = document.querySelectorAll('.fleet-item');
            items.forEach(item => {
                if (category === 'all' || item.classList.contains(category)) {
                    item.style.display = 'flex';
                } else {
                    item.style.display = 'none';
                }
            });
        }

        // Fleet Details Modal Dynamic Populator
        function openFleetModal(model, range, speed, pass, details) {
            document.getElementById('modalTitle').innerText = model;
            document.getElementById('modalSub').innerText = `Range: ${range} | Speed: ${speed}`;
            document.getElementById('modalContent').innerHTML = `
                <div class="space-y-3">
                    <p class="text-gold-300 font-semibold">Capacity: <span class="text-white">${pass}</span></p>
                    <p class="text-gray-300 leading-relaxed">${details}</p>
                    <div class="pt-4 border-t border-gold-400/20">
                        <button onclick="toggleModal('charterModal')" class="w-full py-3 bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-xl">
                            Book ${model}
                        </button>
                    </div>
                </div>
            `;
            toggleModal('charterModal');
        }

        // Customizer Controls Logic
        function setCustomizerAmbiance(type) {
            const bg = document.getElementById('previewBackground');
            const tag = document.getElementById('activeAmbianceTag');
            const title = document.getElementById('previewTitle');
            const desc = document.getElementById('previewDesc');

            document.querySelectorAll('.ambiance-btn').forEach(btn => btn.classList.remove('border-gold-400', 'bg-gold-400/20', 'text-white'));
            event.target.classList.add('border-gold-400', 'bg-gold-400/20', 'text-white');

            if (type === 'sunset') {
                bg.style.backgroundImage = "url('https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?auto=format&fit=crop&w=1200&q=80')";
                tag.innerText = "Sunset Amber Ambiance";
                title.innerText = "Executive Lounge Suite";
                desc.innerText = "Relaxing warm amber circadian lighting designed to minimize jet lag over long-haul oceanic flights.";
            } else if (type === 'midnight') {
                bg.style.backgroundImage = "url('https://images.unsplash.com/photo-1583416750470-965b2707b355?auto=format&fit=crop&w=1200&q=80')";
                tag.innerText = "Midnight Blue Starlight";
                title.innerText = "Private Master Bedroom Suite";
                desc.innerText = "Deep indigo ambient starlight ceiling with noise-canceling acoustics for restorative deep sleep.";
            } else {
                bg.style.backgroundImage = "url('https://images.unsplash.com/photo-1520437358207-323b43b50729?auto=format&fit=crop&w=1200&q=80')";
                tag.innerText = "Zen Daylight Ambiance";
                title.innerText = "Executive Conference Suite";
                desc.innerText = "Full spectrum natural daylight simulation engineered for active board meetings and high-focus work.";
            }
        }

        function updateCustomizerCatering() {
            const select = document.getElementById('cateringSelect');
            const tag = document.getElementById('activeCateringTag');
            tag.innerText = select.options[select.selectedIndex].text;
        }

        // Hero Flight Form Handler
        function handleHeroSearch(e) {
            e.preventDefault();
            alertModal('Flight Search Dispatched', 'Searching live global fleet availability. Your personal aviation manager is preparing your custom quote options.');
        }

        function handleInquirySubmit(e) {
            e.preventDefault();
            alertModal('Inquiry Received', 'Thank you for contacting Aureus Jets. A Senior Charter Advisor has been assigned to your request and will reach out via your preferred channel shortly.');
        }

        function submitModalQuote() {
            toggleModal('charterModal');
            alertModal('Request Confirmed', 'Your jet request has been placed in priority dispatch status.');
        }

        function setFlightType(type) {
            document.getElementById('typeOneWay').className = 'px-4 py-2 rounded-full text-gray-300 hover:text-gold-300 transition-all';
            document.getElementById('typeRoundTrip').className = 'px-4 py-2 rounded-full text-gray-300 hover:text-gold-300 transition-all';
            document.getElementById('typeMultiLeg').className = 'px-4 py-2 rounded-full text-gray-300 hover:text-gold-300 transition-all';

            if(type === 'oneWay') document.getElementById('typeOneWay').className = 'px-4 py-2 rounded-full bg-gold-400 text-obsidian transition-all font-bold';
            if(type === 'roundTrip') document.getElementById('typeRoundTrip').className = 'px-4 py-2 rounded-full bg-gold-400 text-obsidian transition-all font-bold';
            if(type === 'multiLeg') document.getElementById('typeMultiLeg').className = 'px-4 py-2 rounded-full bg-gold-400 text-obsidian transition-all font-bold';
        }

        // Custom Alert Modal Replacement
        function alertModal(title, message) {
            document.getElementById('modalTitle').innerText = title;
            document.getElementById('modalSub').innerText = 'Aureus Global Operations';
            document.getElementById('modalContent').innerHTML = `
                <p class="text-gray-300 leading-relaxed">${message}</p>
                <button onclick="toggleModal('charterModal')" class="w-full py-3 bg-gold-gradient text-obsidian font-bold text-xs uppercase tracking-widest rounded-xl mt-4">
                    Close
                </button>
            `;
            toggleModal('charterModal');
        }
    </script>
</body>
</html>