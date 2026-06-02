<!DOCTYPE html>
<html lang="zh-TW" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>藍海織夢 ｜ 小琉球極致蔚藍指南 - Lambai Island Travel Guide</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome for Premium Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts - Inter & Noto Sans TC -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Noto+Sans+TC:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        ocean: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            200: '#bae6fd',
                            300: '#7dd3fc',
                            400: '#38bdf8',
                            500: '#0ea5e9',
                            600: '#0284c7',
                            700: '#0369a1',
                            800: '#075985',
                            900: '#0c4a6e',
                            950: '#082f49',
                        },
                        sunset: {
                            50: '#fff7ed',
                            100: '#ffedd5',
                            500: '#f97316',
                            600: '#ea580c',
                            700: '#c2410c',
                        },
                        turtle: {
                            50: '#f0fdf4',
                            100: '#dcfce7',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                        }
                    },
                    fontFamily: {
                        sans: ['Noto Sans TC', 'Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    
    <style>
        /* Custom dynamic transitions and visual enhancements */
        .glass-card {
            background: rgba(255, 255, 255, 0.82);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.4);
        }
        .dark-glass {
            background: rgba(15, 23, 42, 0.85);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .text-gradient {
            background: linear-gradient(135deg, #0ea5e9 0%, #0369a1 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .sunset-gradient {
            background: linear-gradient(135deg, #f97316 0%, #db2777 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Smooth Scrollbar Customization */
        ::-webkit-scrollbar {
            width: 10px;
            height: 10px;
        }
        ::-webkit-scrollbar-track {
            background: #f8fafc;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 9999px;
            border: 2px solid #f8fafc;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #0ea5e9;
        }
        
        /* Floating Animation for Sea Turtles */
        @keyframes float {
            0% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-10px) rotate(2deg); }
            100% { transform: translateY(0px) rotate(0deg); }
        }
        .turtle-float {
            animation: float 6s ease-in-out infinite;
        }

        /* Wave Shimmer Effect */
        @keyframes wave-shimmer {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .wave-bg {
            background: linear-gradient(-45deg, #0c4a6e, #075985, #0ea5e9, #1e3a8a);
            background-size: 400% 400%;
            animation: wave-shimmer 15s ease infinite;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans antialiased overflow-x-hidden">

    <!-- Toast Notification Box for interacting without alerts -->
    <div id="toastBox" class="fixed bottom-5 right-5 z-50 transform translate-y-20 opacity-0 transition-all duration-300 ease-out pointer-events-none">
        <div class="bg-slate-900 text-white px-6 py-4 rounded-2xl shadow-2xl flex items-center space-x-3 border border-slate-700/60 max-w-sm">
            <span id="toastIcon" class="text-ocean-400 text-xl"><i class="fas fa-info-circle"></i></span>
            <span id="toastMsg" class="font-medium text-xs sm:text-sm">歡迎來到小琉球極致藍海指南！</span>
        </div>
    </div>

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 w-full z-40 transition-all duration-300 bg-transparent" id="mainNav">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <div class="flex items-center">
                    <a href="#" class="flex items-center space-x-2">
                        <span class="w-10 h-10 bg-ocean-500 rounded-xl flex items-center justify-center text-white shadow-lg shadow-ocean-500/30">
                            <i class="fa-solid fa-umbrella-beach text-lg"></i>
                        </span>
                        <span class="text-lg sm:text-xl font-bold tracking-wider text-white transition-colors duration-300" id="navLogoText">藍海織夢 ｜ 小琉球</span>
                    </a>
                </div>
                <!-- Desktop Menu -->
                <div class="hidden lg:flex items-center space-x-1 lg:space-x-3">
                    <a href="#traffic" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">交通 & 租車</a>
                    <a href="#stay" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">精選宿所</a>
                    <a href="#spots" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">秘境景點</a>
                    <a href="#food" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">島民美食</a>
                    <a href="#activities" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">水上與微醺</a>
                    <a href="#itinerary" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">完美日程</a>
                    <a href="#planner-tool" class="px-3 py-2 rounded-lg text-xs lg:text-sm font-medium text-white hover:text-ocean-200 transition-colors">預算 & 證書</a>
                    <a href="#planner-tool" class="bg-ocean-500 hover:bg-ocean-600 text-white px-4 py-2 rounded-full text-xs lg:text-sm font-semibold shadow-md hover:shadow-lg transition-all transform hover:-translate-y-0.5">預算助手</a>
                </div>
                <!-- Mobile Menu Button -->
                <div class="lg:hidden flex items-center">
                    <button id="mobileMenuBtn" class="text-white hover:text-ocean-200 focus:outline-none p-2 rounded-lg" aria-label="Toggle Menu">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Drawer -->
        <div id="mobileDrawer" class="hidden lg:hidden bg-slate-900/95 backdrop-blur-lg border-b border-slate-800 px-4 pt-2 pb-6 space-y-2">
            <a href="#traffic" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">交通 & 租車</a>
            <a href="#stay" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">精選宿所</a>
            <a href="#spots" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">秘境景點</a>
            <a href="#food" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">島民美食</a>
            <a href="#activities" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">水上與微醺</a>
            <a href="#itinerary" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">完美日程</a>
            <a href="#planner-tool" class="block px-3 py-2 rounded-lg text-base font-medium text-white hover:bg-slate-800" onclick="closeDrawer()">預算與證書</a>
            <a href="#planner-tool" class="block bg-ocean-500 text-center text-white px-4 py-2 rounded-xl text-base font-semibold" onclick="closeDrawer()">預算助手</a>
        </div>
    </nav>

    <!-- Hero Header -->
    <div class="relative h-screen flex items-center justify-center overflow-hidden">
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?auto=format&fit=crop&w=1920&q=80" 
                 alt="小琉球蔚藍大海與海龜" 
                 class="w-full h-full object-cover brightness-[0.4] transform scale-105 transition-transform duration-1000"
                 id="heroBg"
                 onerror="this.src='https://placehold.co/1920x1080/0284c7/ffffff?text=Beautiful+Xiao+Liu+Qiu'">
        </div>
        
        <!-- Animated Wave Overlay -->
        <div class="absolute bottom-0 left-0 w-full overflow-hidden leading-[0] z-10">
            <svg viewBox="0 0 1200 120" preserveAspectRatio="none" class="relative block w-full h-[60px] text-slate-50 fill-current">
                <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V120H0V0C26.9,3.56,57.14,14,88.43,26.65,152.42,52.42,217.16,68.7,321.39,56.44Z"></path>
            </svg>
        </div>

        <!-- Float Green Turtle Vector Asset over Hero -->
        <div class="absolute right-4 bottom-24 md:right-20 md:bottom-32 z-10 w-28 h-28 sm:w-44 sm:h-44 opacity-80 turtle-float pointer-events-none">
            <svg viewBox="0 0 512 512" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-full h-full drop-shadow-[0_10px_15px_rgba(34,197,94,0.3)]">
                <path d="M256 64C230 64 200 80 180 110C195 125 215 130 230 130C235 120 245 110 256 110C267 110 277 120 282 130C297 130 317 125 332 110C312 80 282 64 256 64Z" fill="#15803d"/>
                <path d="M256 128C150 128 112 180 112 280C112 370 160 400 256 400C352 400 400 370 400 280C400 180 362 128 256 128Z" fill="#166534"/>
                <path d="M256 148C170 148 132 190 132 280C132 350 170 380 256 380C342 380 380 350 380 280C380 190 342 148 256 148Z" fill="#22c55e"/>
                <path d="M256 180L210 220L220 270L256 250L292 270L302 220L256 180Z" fill="#14532d"/>
                <path d="M112 200C70 200 48 240 48 260C48 290 80 290 96 280" stroke="#15803d" stroke-width="16" stroke-linecap="round"/>
                <path d="M400 200C442 200 464 240 464 260C464 290 432 290 416 280" stroke="#15803d" stroke-width="16" stroke-linecap="round"/>
                <path d="M130 360C90 380 80 420 90 440C110 440 130 420 140 390" stroke="#15803d" stroke-width="16" stroke-linecap="round"/>
                <path d="M382 360C422 380 432 420 422 440C402 440 382 420 372 390" stroke="#15803d" stroke-width="16" stroke-linecap="round"/>
            </svg>
        </div>

        <!-- Hero Content -->
        <div class="relative z-20 max-w-5xl mx-auto px-4 text-center mt-12">
            <span class="inline-flex items-center space-x-2 bg-ocean-500/20 text-ocean-300 border border-ocean-500/30 px-4 py-1.5 rounded-full text-xs sm:text-sm font-semibold mb-6 uppercase tracking-widest animate-pulse">
                <i class="fa-solid fa-location-dot text-emerald-400"></i>
                <span>探索台灣最美的零碳珊瑚度假島</span>
            </span>
            <h1 class="text-4xl sm:text-6xl md:text-7xl font-extrabold text-white tracking-tight leading-none mb-6">
                藍海織夢 <span class="text-transparent bg-clip-text bg-gradient-to-r from-ocean-300 via-emerald-300 to-amber-300">小琉球極致蔚藍</span>
            </h1>
            <p class="text-base sm:text-xl md:text-2xl text-slate-200 max-w-3xl mx-auto font-light mb-10 leading-relaxed">
                與綠蠵龜攜手同共游、踏足如翡翠果凍般透徹的白沙秘境。一場融合絕美落日、隱藏美食與慵懶微醺的夢幻小島行旅，正等著你一鍵打包。
            </p>

            <!-- Quick Action Finder -->
            <div class="glass-card p-3 sm:p-5 rounded-3xl max-w-3xl mx-auto shadow-2xl transition-all hover:shadow-ocean-500/20">
                <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                    <button onclick="scrollToId('spots')" class="flex items-center space-x-3 p-3 rounded-2xl hover:bg-ocean-100/50 transition-colors text-left group">
                        <div class="w-10 h-10 bg-ocean-100 group-hover:bg-ocean-200 text-ocean-600 rounded-xl flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-compass text-lg"></i>
                        </div>
                        <div>
                            <p class="text-[10px] text-slate-400 font-semibold uppercase">Must See</p>
                            <p class="text-xs sm:text-sm font-bold text-slate-700">探索必訪與隱密秘境</p>
                        </div>
                    </button>
                    
                    <button onclick="scrollToId('food')" class="flex items-center space-x-3 p-3 rounded-2xl hover:bg-emerald-50/50 transition-colors text-left group">
                        <div class="w-10 h-10 bg-emerald-100 group-hover:bg-emerald-200 text-emerald-600 rounded-xl flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-utensils text-lg"></i>
                        </div>
                        <div>
                            <p class="text-[10px] text-slate-400 font-semibold uppercase">Local Food</p>
                            <p class="text-xs sm:text-sm font-bold text-slate-700">饕客與島民口袋美食</p>
                        </div>
                    </button>

                    <button onclick="scrollToId('planner-tool')" class="flex items-center space-x-3 p-3 rounded-2xl hover:bg-amber-50/50 transition-colors text-left group">
                        <div class="w-10 h-10 bg-amber-100 group-hover:bg-amber-200 text-amber-600 rounded-xl flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-passport text-lg"></i>
                        </div>
                        <div>
                            <p class="text-[10px] text-slate-400 font-semibold uppercase">Interactive Tool</p>
                            <p class="text-xs sm:text-sm font-bold text-slate-700">預算估算與守護者證書</p>
                        </div>
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Tide & Weather Forecast Simulator (New Interactive Block) -->
    <section class="py-12 bg-white border-b border-slate-100 relative z-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-gradient-to-r from-ocean-50 to-emerald-50 rounded-3xl p-6 border border-ocean-100 shadow-sm grid grid-cols-1 md:grid-cols-4 gap-6 items-center">
                <div class="md:col-span-1 text-center md:text-left">
                    <span class="bg-ocean-100 text-ocean-700 px-3 py-1 rounded-full text-xs font-semibold">小島天氣與海龜預報</span>
                    <h3 class="text-xl font-bold text-slate-800 mt-2">今日海況即時指數</h3>
                    <p class="text-xs text-slate-500 mt-1">即時海溫、潮汐變化與尋訪綠蠵龜最佳時光預測。</p>
                </div>
                <!-- Weather Simulator Card -->
                <div class="bg-white p-4 rounded-2xl border border-slate-100 shadow-sm flex items-center space-x-4">
                    <span class="w-12 h-12 rounded-xl bg-amber-100 text-amber-500 flex items-center justify-center text-2xl"><i class="fa-solid fa-sun"></i></span>
                    <div>
                        <p class="text-xs text-slate-400">當前溫度 / 水溫</p>
                        <p class="text-base font-bold text-slate-800">29.5 °C <span class="text-xs text-ocean-500">/ 26.2°C</span></p>
                        <p class="text-[10px] text-emerald-600 font-medium"><i class="fa-solid fa-circle-check"></i> 超好下水水溫</p>
                    </div>
                </div>
                <!-- Tide Card -->
                <div class="bg-white p-4 rounded-2xl border border-slate-100 shadow-sm flex items-center space-x-4">
                    <span class="w-12 h-12 rounded-xl bg-blue-100 text-blue-500 flex items-center justify-center text-2xl"><i class="fa-solid fa-water"></i></span>
                    <div>
                        <p class="text-xs text-slate-400">當前潮汐狀態</p>
                        <p class="text-base font-bold text-slate-800" id="tideText">乾潮 (低潮期)</p>
                        <p class="text-[10px] text-slate-500" id="tideSubText">秘境果凍海與潮間帶最佳探索期！</p>
                    </div>
                </div>
                <!-- Turtle Index Card -->
                <div class="bg-white p-4 rounded-2xl border border-slate-100 shadow-sm flex items-center space-x-4">
                    <span class="w-12 h-12 rounded-xl bg-green-100 text-green-600 flex items-center justify-center text-2xl animate-bounce"><i class="fa-solid fa-turtle"></i></span>
                    <div>
                        <p class="text-xs text-slate-400">海龜出沒活躍率</p>
                        <p class="text-base font-bold text-emerald-600">95% (極高)</p>
                        <p class="text-[10px] text-slate-500">推薦地點：花瓶岩 & 美人洞</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Traffic & Transport section -->
    <section id="traffic" class="py-20 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-slate-900 tracking-tight">登島戰略：如何輕鬆順利抵達？</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-500 mt-4 text-sm sm:text-base">從本島南下，再轉搭快艇出海。我們為您整理了最流暢的船票指引與在地靠譜的車行名單。</p>
            </div>

            <!-- Steps Tabs -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                <!-- Step 1: Land Transportation -->
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl hover:-translate-y-1 transition-all duration-300">
                    <span class="w-12 h-12 rounded-2xl bg-ocean-100 text-ocean-600 flex items-center justify-center text-xl font-bold mb-6">01</span>
                    <h3 class="text-lg sm:text-xl font-bold text-slate-900 mb-4"><i class="fa-solid fa-train mr-2 text-ocean-500"></i>抵達屏東東港碼頭</h3>
                    <ul class="space-y-3.5 text-slate-600 text-xs sm:text-sm">
                        <li class="flex items-start">
                            <span class="text-emerald-500 mr-2 mt-1"><i class="fa-solid fa-circle-check"></i></span>
                            <span><strong>高鐵：</strong>搭至左營站，轉乘「台灣好行大鵬灣琉球線」客運或叫共乘計程車直達東港碼頭。</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-emerald-500 mr-2 mt-1"><i class="fa-solid fa-circle-check"></i></span>
                            <span><strong>台鐵：</strong>搭至屏東站或高雄站，轉乘屏東客運/港都巴士往東港方向。</span>
                        </li>
                        <li class="flex items-start">
                            <span class="text-emerald-500 mr-2 mt-1"><i class="fa-solid fa-circle-check"></i></span>
                            <span><strong>自行開車：</strong>導航至東港鹽埔漁港，碼頭周邊有許多付費室內/室外過夜停車場（約 $150-200/天）。</span>
                        </li>
                    </ul>
                </div>

                <!-- Step 2: Ferry Info -->
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl hover:-translate-y-1 transition-all duration-300">
                    <span class="w-12 h-12 rounded-2xl bg-ocean-100 text-ocean-600 flex items-center justify-center text-xl font-bold mb-6">02</span>
                    <h3 class="text-lg sm:text-xl font-bold text-slate-900 mb-4"><i class="fa-solid fa-ship mr-2 text-ocean-500"></i>東港 ⇄ 小琉球渡輪</h3>
                    <p class="text-slate-500 text-xs mb-3">船程約 25 - 30 分鐘，主要分為公營與民營船，大部分民宿套票皆搭配民營船，船班極為穩定。</p>
                    <div class="bg-slate-50 p-4 rounded-2xl space-y-2 text-xs mb-4 border border-slate-100">
                        <p class="flex justify-between"><strong>泰富航運：</strong><span class="text-slate-600">東港 ⇄ 白沙尾港 (極新、班次密)</span></p>
                        <p class="flex justify-between"><strong>藍白航運：</strong><span class="text-slate-600">東港 ⇄ 白沙尾港 (設計感足、舒適)</span></p>
                        <p class="flex justify-between"><strong>大福航運：</strong><span class="text-slate-600">鹽埔 ⇄ 大福漁港 (適合自駕車託運)</span></p>
                    </div>
                    <ul class="space-y-2 text-slate-600 text-xs">
                        <li><i class="fa-regular fa-clock mr-1 text-ocean-500"></i> 營運時間：07:00 - 17:00（每 1 ~ 1.5 小時一班，假日視人潮機動加開加班船）</li>
                        <li><i class="fa-solid fa-ticket mr-1 text-ocean-500"></i> 來回票價：全票約 NT$410 - $450（強烈建議買來回票較划算）</li>
                    </ul>
                </div>

                <!-- Step 3: Scooter Rental -->
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 hover:shadow-xl hover:-translate-y-1 transition-all duration-300">
                    <span class="w-12 h-12 rounded-2xl bg-ocean-100 text-ocean-600 flex items-center justify-center text-xl font-bold mb-6">03</span>
                    <h3 class="text-lg sm:text-xl font-bold text-slate-900 mb-4"><i class="fa-solid fa-motorcycle mr-2 text-ocean-500"></i>島上通行：優質機車出租</h3>
                    <p class="text-slate-500 text-xs sm:text-sm mb-4">小琉球地勢多陡坡與彎道，機車是最便利的探險載具。強烈推薦選擇無噪音、低排碳的電動車，為島嶼減碳！</p>
                    
                    <div class="space-y-3">
                        <div class="border-l-4 border-emerald-500 pl-3">
                            <p class="text-xs sm:text-sm font-bold text-slate-800">晴天聯盟・低碳電動機車</p>
                            <p class="text-[11px] text-slate-500">全新智能電車，無引擎熱氣與噪音。全島多個電池交換點，費用約 $400 - $500/天。</p>
                        </div>
                        <div class="border-l-4 border-ocean-500 pl-3">
                            <p class="text-xs sm:text-sm font-bold text-slate-800">尚美機車出租 (白沙港口旁)</p>
                            <p class="text-[11px] text-slate-500">出碼頭步行 1 分鐘即達，燃油車況新，保養優良，附兩頂安全帽，約 $350 - $400/天。</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Island Explorer & Hotspot Map -->
    <section class="py-20 bg-gradient-to-br from-ocean-900 to-slate-950 text-white relative overflow-hidden">
        <div class="absolute inset-0 bg-[radial-gradient(circle_at_30%_30%,rgba(14,165,233,0.15),transparent_50%)]"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <span class="bg-ocean-500/20 text-ocean-300 border border-ocean-500/30 px-3 py-1 rounded-full text-xs font-semibold uppercase tracking-wider">Geographic Guide</span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-white mt-4">一條公路，環島收服整座蔚藍</h2>
                    <p class="text-slate-300 text-sm sm:text-base leading-relaxed mt-4">
                        小琉球環島公路全長約 18 公里，騎機車不中斷繞一圈只需約 30 分鐘。隨意按按右方的**「極致環島互動微地圖」**，就能搶先探訪各方位景點特性與海龜、落日觀賞重點！
                    </p>
                    
                    <div class="mt-6 p-5 bg-slate-900/60 rounded-2xl border border-slate-800 space-y-4">
                        <p class="text-xs text-slate-300 flex items-start">
                            <span class="text-ocean-400 mr-3 text-sm"><i class="fa-solid fa-umbrella-beach"></i></span>
                            <span><strong>西北海岸線：</strong>多為驚險奇峭的珊瑚石灰岩峽谷地貌，是觀看海龜呼吸、地層變動的經典自然風景帶。</span>
                        </p>
                        <p class="text-xs text-slate-300 flex items-start">
                            <span class="text-amber-400 mr-3 text-sm"><i class="fa-solid fa-sun"></i></span>
                            <span><strong>西南與東南方：</strong>擁有全島最無死角的湛藍海平線，是迎接日出與送走夕陽的絕美黃金觀景平台。</span>
                        </p>
                    </div>
                </div>

                <!-- CSS SVG Interactive Map Panel -->
                <div class="relative bg-slate-900/40 rounded-3xl p-6 border border-slate-800 flex flex-col justify-between h-[420px]">
                    <div class="text-center">
                        <h4 class="text-xs font-bold text-slate-400 uppercase tracking-widest">Interactive Live Map</h4>
                        <h3 class="text-base font-bold text-white mt-1">✨ 點選地圖地標・模擬線上環島 ✨</h3>
                        <p id="mapInfoText" class="text-xs text-ocean-300 mt-2 font-medium">請在下方虛擬羅盤地圖上，點選任何熱點地標！</p>
                    </div>

                    <!-- Abstract Interactive Micro-Map Canvas Mockup -->
                    <div class="relative w-full max-w-sm mx-auto h-56 my-4 flex items-center justify-center">
                        <!-- Abstract Soft Glowing Island Shape in SVG -->
                        <svg viewBox="0 0 400 240" class="absolute w-full h-full opacity-30 pointer-events-none">
                            <path d="M 80,120 Q 120,40 220,60 T 320,120 T 260,190 T 120,180 Z" fill="none" stroke="#0ea5e9" stroke-width="4" stroke-dasharray="8 4" />
                            <path d="M 90,130 Q 130,50 210,70 T 310,130 T 250,180 T 130,170 Z" fill="#0ea5e9" opacity="0.1" />
                        </svg>

                        <!-- Pointers layered on top with absolute positioning relative to 400x240 canvas -->
                        <!-- North: Vase Rock -->
                        <button onclick="showMapPin('花瓶岩 & 白沙尾港 (正北側)', '小島最重要的門戶港口！緊鄰清澈水域，旁邊就是白沙沙灘，早晨跟黃昏是目睹海龜探頭換氣機率最高的黃金點。')" class="absolute top-2 left-1/2 transform -translate-x-1/2 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-sky-400 border-2 border-sky-500/50 flex items-center justify-center hover:bg-sky-500 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-anchor text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">北部：白沙尾港</span>
                        </button>

                        <!-- Northwest: Beauty Cave -->
                        <button onclick="showMapPin('美人洞景區 (西北側)', '壯麗的珊瑚礁石灰岩步道，海景極其寬廣。居高臨下俯瞰，海水清澈如洗，常能看見十幾隻海龜同時在海面上游泳！')" class="absolute top-12 left-16 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-emerald-400 border-2 border-emerald-500/50 flex items-center justify-center hover:bg-emerald-500 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-location-pin text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">西北：美人洞</span>
                        </button>

                        <!-- Center: Wild Boar Trench -->
                        <button onclick="showMapPin('山豬溝天然步道 (島中央)', '深藏在珊瑚礁縫隙間的天然熱帶雨林，密布高大的筆筒樹與滿牆生長綠色蕨類。宛如電影侏羅紀公園的原始森林景象，乘涼消暑極致神地。')" class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-emerald-500 border-2 border-emerald-400/50 flex items-center justify-center hover:bg-emerald-400 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-tree text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">島中央：山豬溝</span>
                        </button>

                        <!-- Southwest: Sunset Pavilion -->
                        <button onclick="showMapPin('落日亭 (西南側)', '直接面對毫無死角的大海平線，是捕捉火紅太陽沒入巴士海峽的絕佳地標。在海風吹拂下，晚霞會將天空與海洋渲染成神仙紫粉色。')" class="absolute bottom-10 left-12 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-orange-400 border-2 border-orange-500/50 flex items-center justify-center hover:bg-orange-500 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-sun text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">西南：落日亭</span>
                        </button>

                        <!-- Southeast: Thick Reef & Sunrise -->
                        <button onclick="showMapPin('厚石裙礁 & 旭日亭 (東南側)', '擁有百褶裙般壯麗的海蝕珊瑚礁平台，裙擺凹槽形成無風無浪的「天然翠綠果凍海」。隔壁的旭日亭則是迎接萬道金色曙光的第一首選。')" class="absolute bottom-6 right-16 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-pink-400 border-2 border-pink-500/50 flex items-center justify-center hover:bg-pink-500 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-umbrella-beach text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">東南：厚石秘境</span>
                        </button>

                        <!-- East: Dafu Port & Wildwood -->
                        <button onclick="showMapPin('網美老木 & 大福漁港 (正東側)', '大福港旁消波塊深處藏有一條卡在海邊巨石上的漂流木。坐在上面，襯著後方寶藍色海浪，是 IG 人氣最高的秘境拍攝點。')" class="absolute top-1/2 right-10 transform -translate-y-1/2 group">
                            <span class="w-10 h-10 rounded-full bg-slate-800 text-yellow-400 border-2 border-yellow-500/50 flex items-center justify-center hover:bg-yellow-500 hover:text-white transition-all shadow-lg hover:scale-110">
                                <i class="fa-solid fa-compass text-sm"></i>
                            </span>
                            <span class="absolute bottom-full mb-2 left-1/2 transform -translate-x-1/2 scale-0 group-hover:scale-100 bg-slate-900 text-[10px] px-2 py-1 rounded-lg transition-all text-white font-bold whitespace-nowrap z-20 shadow-md">東部：網美老木</span>
                        </button>
                    </div>

                    <!-- Map Detail Panel Feedback -->
                    <div id="mapDetailPanel" class="bg-slate-950/80 p-3 sm:p-4 rounded-2xl border border-slate-800 text-center text-xs text-slate-300 transition-all">
                        💡 提示：點點看上方羅盤點，解鎖對應景區的私房驚喜介紹喔！
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Accommodation Lodges Section -->
    <section id="stay" class="py-20 bg-slate-900 text-white relative">
        <div class="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1920&q=80')] bg-cover bg-center opacity-5"></div>
        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold tracking-tight">枕海入眠：精選小島夢幻宿所</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-400 mt-4 text-sm sm:text-base">我們挑選了口碑極佳、風格各異的頂級旅宿，從北歐質感、異國摩洛哥到峇里島莊園，滿足您的挑剔美學。</p>
            </div>

            <!-- Accommodations Grid -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Hotel 1 -->
                <div class="dark-glass rounded-3xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group shadow-lg">
                    <div class="h-64 overflow-hidden relative">
                        <img src="https://images.unsplash.com/photo-1566073771259-6a8506099945?auto=format&fit=crop&w=800&q=80" alt="朵小路北歐民宿" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/0284c7/ffffff?text=Duoxiaolu+Villa'">
                        <span class="absolute top-4 right-4 bg-ocean-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow-md">文青首選</span>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center justify-between mb-3">
                            <span class="text-xs text-ocean-300 tracking-wider uppercase font-semibold">極簡北歐風 ｜ 附電梯</span>
                            <div class="flex items-center text-amber-400 text-xs font-bold">
                                <i class="fa-solid fa-star mr-1"></i>4.8
                            </div>
                        </div>
                        <h3 class="text-xl font-bold mb-2">朵小路北歐民宿</h3>
                        <p class="text-slate-400 text-xs mb-4 leading-relaxed line-clamp-3">
                            全島少數附有電梯的貼心設計，北歐輕白與溫潤木質調交織。每天早晨提供美味豐盛的手作特色餐點，民宿內有多款網美拍照旋轉木馬，特別適合家庭與質感旅客。
                        </p>
                        <div class="border-t border-slate-800/80 pt-4 flex justify-between items-center text-xs text-slate-400">
                            <span><i class="fa-solid fa-location-dot mr-1 text-ocean-400"></i>琉球鄉復興路163-2號</span>
                            <span class="text-ocean-400 font-bold text-sm">約 NT$ 3,200 起</span>
                        </div>
                    </div>
                </div>

                <!-- Hotel 2 -->
                <div class="dark-glass rounded-3xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group shadow-lg">
                    <div class="h-64 overflow-hidden relative">
                        <img src="https://images.unsplash.com/photo-1540555700478-4be289fbecef?auto=format&fit=crop&w=800&q=80" alt="尊順祿藝術旅店" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/ea580c/ffffff?text=Zunshunlu+Art+Hotel'">
                        <span class="absolute top-4 right-4 bg-amber-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow-md">頂級奢華</span>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center justify-between mb-3">
                            <span class="text-xs text-amber-400 tracking-wider uppercase font-semibold">摩洛哥奇幻風 ｜ 獨立泳池</span>
                            <div class="flex items-center text-amber-400 text-xs font-bold">
                                <i class="fa-solid fa-star mr-1"></i>4.9
                            </div>
                        </div>
                        <h3 class="text-xl font-bold mb-2">尊順祿藝術旅店</h3>
                        <p class="text-slate-400 text-xs mb-4 leading-relaxed line-clamp-3">
                            外觀極具強烈馬賽克磁磚美學，大膽拼貼幾何美感。頂級房型配有私人戶外冷熱水池與純白超大浴缸。極度推薦給情侶、蜜月 or 追求極致異國奢華感的小島享樂主義者。
                        </p>
                        <div class="border-t border-slate-800/80 pt-4 flex justify-between items-center text-xs text-slate-400">
                            <span><i class="fa-solid fa-location-dot mr-1 text-amber-400"></i>小琉球本漁路160巷</span>
                            <span class="text-amber-400 font-bold text-sm">約 NT$ 4,800 起</span>
                        </div>
                    </div>
                </div>

                <!-- Hotel 3 -->
                <div class="dark-glass rounded-3xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group shadow-lg">
                    <div class="h-64 overflow-hidden relative">
                        <img src="https://images.unsplash.com/photo-1499793983690-e29da59ef1c2?auto=format&fit=crop&w=800&q=80" alt="輪廓莊園" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" onerror="this.src='https://placehold.co/600x400/10b981/ffffff?text=Outline+Manor'">
                        <span class="absolute top-4 right-4 bg-emerald-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow-md">南洋海景</span>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center justify-between mb-3">
                            <span class="text-xs text-emerald-400 tracking-wider uppercase font-semibold">峇里島莊園風 ｜ 慵懶發呆亭</span>
                            <div class="flex items-center text-amber-400 text-xs font-bold">
                                <i class="fa-solid fa-star mr-1"></i>4.7
                            </div>
                        </div>
                        <h3 class="text-xl font-bold mb-2">輪廓莊園</h3>
                        <p class="text-slate-400 text-xs mb-4 leading-relaxed line-clamp-3">
                            一秒飛抵峇里島！占地寬廣，擁有蓊鬱的棕櫚椰林與發呆亭中庭。房內挑高舒適、通透明亮，清晨陽光透過落地窗灑下，能徹底洗去都市累積的喧囂與心靈疲憊。
                        </p>
                        <div class="border-t border-slate-800/80 pt-4 flex justify-between items-center text-xs text-slate-400">
                            <span><i class="fa-solid fa-location-dot mr-1 text-emerald-400"></i>琉球鄉復興路163-5號</span>
                            <span class="text-emerald-400 font-bold text-sm">約 NT$ 3,600 起</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Secret Spots & Filter Section -->
    <section id="spots" class="py-20 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-slate-900 tracking-tight">小琉球絕美秘境與經典景點</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-500 mt-4 text-sm sm:text-base">點選分類按鈕，過濾我們為您深入蒐集的地標景點，不論是經典打卡或私房果凍海秘境一覽無遺。</p>
                
                <!-- Filter buttons (Passing 'event' explicitly now to guarantee Safari & Firefox safety) -->
                <div class="flex flex-wrap justify-center gap-2 mt-8">
                    <button onclick="filterSpots('all', event)" class="spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-ocean-500 text-white shadow-md transition-all">顯示全部</button>
                    <button onclick="filterSpots('must', event)" class="spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-white text-slate-600 hover:bg-slate-100 transition-all shadow-sm border border-slate-200">經典地標</button>
                    <button onclick="filterSpots('secret', event)" class="spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-white text-slate-600 hover:bg-slate-100 transition-all shadow-sm border border-slate-200">私房秘境</button>
                    <button onclick="filterSpots('sun', event)" class="spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-white text-slate-600 hover:bg-slate-100 transition-all shadow-sm border border-slate-200">極美晨昏</button>
                </div>
            </div>

            <!-- Spot Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8" id="spotContainer">
                <!-- Spot 1: Vase Rock -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="must">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1505118380757-91f5f5632de0?auto=format&fit=crop&w=800&q=80" alt="花瓶岩" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/0ea5e9/ffffff?text=Vase+Rock'">
                        <span class="absolute top-4 left-4 bg-sky-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">經典地標</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">花瓶岩 (Vase Rock)</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            小琉球最著名的地標礁石，因地殼抬升加上海水侵蝕而成。頂部生長著蔥鬱植物，神似插著鮮花的花瓶。周邊海水極清，是全島海龜出現最頻繁的浮潛聖地。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-sky-500"></i>鄰近白沙尾港口，騎車/步行 5 分鐘即達。
                        </div>
                    </div>
                </div>

                <!-- Spot 2: Driftwood Secret -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="secret">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1473116763269-255415b9ff22?auto=format&fit=crop&w=800&q=80" alt="網美老木" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/10b981/ffffff?text=Driftwood+Secret'">
                        <span class="absolute top-4 left-4 bg-emerald-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">熱門秘境</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">大福港旁・網美老木</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            卡在岸邊珊瑚巨石間的一根巨大漂流木。旅人可坐在漂流木上，迎風眺望波瀾壯闊的寶藍色海面，畫面寧靜、孤寂，是近年網紅必訪打卡頂級秘地。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-emerald-500"></i>大福港堤防旁，需沿消波塊小徑步行 5 分鐘。
                        </div>
                    </div>
                </div>

                <!-- Spot 3: Sunset Pavilion -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="sun">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="落日亭" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/f97316/ffffff?text=Sunset+Pavilion'">
                        <span class="absolute top-4 left-4 bg-orange-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">最美日落</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">落日亭 (Sunset Pavilion)</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            座落在小琉球西南角的珊瑚礁高台。面前是無遮蔽的蔚藍大海。每到傍晚，整顆通紅落日會在金黃色光暈下緩緩沒入地平線，渲染整片汪洋。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-orange-500"></i>小島西南端環島公路旁。
                        </div>
                    </div>
                </div>

                <!-- Spot 4: Sunrise Pavilion -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="sun">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1470252649378-9c29740c9fa8?auto=format&fit=crop&w=800&q=80" alt="旭日亭" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/f59e0b/ffffff?text=Sunrise+Pavilion'">
                        <span class="absolute top-4 left-4 bg-amber-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">震撼日出</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">旭日亭 (Sunrise Pavilion)</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            前身為垃圾焚化場，經改建整理後成為迎曙光的最佳平台。居高臨下，看紅日從海平面與中央山脈輪廓間緩緩升起，灑下萬道刺眼的金黃萬丈光芒。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-amber-500"></i>島東南方海岸，鄰近大福漁港。
                        </div>
                    </div>
                </div>

                <!-- Spot 5: Jelly Sea Reef -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="secret">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1519046904884-53103b34b206?auto=format&fit=crop&w=800&q=80" alt="厚石裙礁" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/10b981/ffffff?text=Jelly+Sea+Secret'">
                        <span class="absolute top-4 left-4 bg-emerald-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">果凍海秘境</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">厚石秘境・天然果凍海泳池</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            隱藏在紅番石與觀音石礁石群之間。海蝕凹槽礁岩擋住了猛烈外海波浪，形成一個波光粼粼、清澈透明度極高的翠綠色泳池，極度適合涉水玩樂。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-emerald-500"></i>沿環島公路厚石裙礁小徑往下走，需穿厚底涼鞋防礁岩割傷。
                        </div>
                    </div>
                </div>

                <!-- Spot 6: Classic Caves -->
                <div class="spot-card bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-100" data-category="must">
                    <div class="h-56 relative overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=800&q=80" alt="美人洞烏鬼洞" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/800x600/0ea5e9/ffffff?text=Island+Classic+Caves'">
                        <span class="absolute top-4 left-4 bg-sky-500 text-white text-xs px-3 py-1 rounded-full font-bold shadow">經典必玩</span>
                    </div>
                    <div class="p-6">
                        <h3 class="text-lg font-bold text-slate-900 mb-2">美人洞、山豬溝、烏鬼洞</h3>
                        <p class="text-slate-600 text-xs sm:text-sm leading-relaxed mb-4">
                            小琉球「三大經典景區」，一票到底暢遊。步道曲折盤旋於鬼斧神工的巨大珊瑚礁石灰岩壁之間，伴隨熱帶盤根錯節的老樹，充滿神秘的原始美感。
                        </p>
                        <div class="text-[11px] text-slate-400 flex items-center">
                            <i class="fa-solid fa-location-dot mr-1.5 text-sky-500"></i>分布於島嶼西北方與西方海岸線。
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Food section -->
    <section id="food" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-slate-900 tracking-tight">舌尖大冒險：小琉球必吃島民美食</h2>
                <div class="h-1.5 w-16 bg-emerald-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-500 mt-4 text-sm sm:text-base">從小島傳統晨光早點、文青感爆棚的海龜雞蛋糕，到入夜後只有在地人才知道的宵夜首選。</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Food Item 1 -->
                <div class="bg-slate-50 rounded-2xl p-6 hover:bg-emerald-50/50 hover:border-emerald-200 transition-all border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-3">
                            <span class="bg-amber-100 text-amber-800 text-[10px] font-extrabold px-2 py-0.5 rounded-full">超長排隊</span>
                            <span class="text-xs text-slate-400">小島晨光</span>
                        </div>
                        <h3 class="text-base font-bold text-slate-900 mb-2">洪媽媽早餐店</h3>
                        <p class="text-xs text-slate-500 mb-4 leading-relaxed">
                            開店三十餘年的早餐傳奇！必點特製外酥內 Q 的「琉球粿」（芋頭/南瓜風味）、造型邪惡爆漿的「賓士包」，晚來真的會搶不完。
                        </p>
                    </div>
                    <div class="text-[11px] text-slate-400 border-t border-slate-200/60 pt-3">
                        <i class="fa-solid fa-location-dot mr-1 text-amber-500"></i>琉球鄉大福村和平路28-5號
                    </div>
                </div>

                <!-- Food Item 2 -->
                <div class="bg-slate-50 rounded-2xl p-6 hover:bg-emerald-50/50 hover:border-emerald-200 transition-all border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-3">
                            <span class="bg-red-100 text-red-800 text-[10px] font-extrabold px-2 py-0.5 rounded-full">老街美味</span>
                            <span class="text-xs text-slate-400">經典麵食</span>
                        </div>
                        <h3 class="text-base font-bold text-slate-900 mb-2">相思麵</h3>
                        <p class="text-xs text-slate-500 mb-4 leading-relaxed">
                            傳承紅磚灶台與純柴火慢煮肉燥，湯頭濃香迷人。淋上店內特製的「相思辣醬」，麻香帶勁，也是伴手禮必帶的高人氣手信。
                        </p>
                    </div>
                    <div class="text-[11px] text-slate-400 border-t border-slate-200/60 pt-3">
                        <i class="fa-solid fa-location-dot mr-1 text-red-500"></i>琉球鄉上杉路31-1號
                    </div>
                </div>

                <!-- Food Item 3 -->
                <div class="bg-slate-50 rounded-2xl p-6 hover:bg-emerald-50/50 hover:border-emerald-200 transition-all border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-3">
                            <span class="bg-emerald-100 text-emerald-800 text-[10px] font-extrabold px-2 py-0.5 rounded-full">島民私藏宵夜</span>
                            <span class="text-xs text-slate-400">罪惡宵夜</span>
                        </div>
                        <h3 class="text-base font-bold text-slate-900 mb-2">小琉球廟口鹹酥雞</h3>
                        <p class="text-xs text-slate-500 mb-4 leading-relaxed">
                            <strong>【隱藏秘境美食】</strong> 在三隆宮廟口前。特調香甜醬汁裹上現炸物，搭配滿滿九層塔與辛辣生蒜，是潛水教練們深夜大推的罪惡消遣。
                        </p>
                    </div>
                    <div class="text-[11px] text-slate-400 border-t border-slate-200/60 pt-3">
                        <i class="fa-solid fa-location-dot mr-1 text-emerald-500"></i>小琉球三隆宮廟口
                    </div>
                </div>

                <!-- Food Item 4 -->
                <div class="bg-slate-50 rounded-2xl p-6 hover:bg-emerald-50/50 hover:border-emerald-200 transition-all border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-3">
                            <span class="bg-pink-100 text-pink-800 text-[10px] font-extrabold px-2 py-0.5 rounded-full">IG 必拍</span>
                            <span class="text-xs text-slate-400">網美下午茶</span>
                        </div>
                        <h3 class="text-base font-bold text-slate-900 mb-2">海龜燒 ＆ 小米甜甜圈</h3>
                        <p class="text-xs text-slate-500 mb-4 leading-relaxed">
                            現烤圓滾滾的海龜造型雞蛋糕，咬開是邪惡爆漿卡士達或起司，配上旁邊熱騰騰外酥內 Q 的現炸小米甜甜圈，拍照、口感都極佳。
                        </p>
                    </div>
                    <div class="text-[11px] text-slate-400 border-t border-slate-200/60 pt-3">
                        <i class="fa-solid fa-location-dot mr-1 text-pink-500"></i>白沙尾港周邊商店街
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Water & Night Activities -->
    <section id="activities" class="py-20 bg-gradient-to-b from-slate-50 to-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-slate-900 tracking-tight">極致體驗：白天海龜共游 ＆ 慵懶微醺夜</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-500 mt-4 text-sm sm:text-base">白天穿梭果凍海追風逐浪，夜晚吹拂著海風點燃微醺氛圍，感受離島最迷人的冰火雙重天。</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- Water Adventures -->
                <div class="bg-white rounded-3xl p-8 shadow-sm border border-slate-100/80">
                    <div class="flex items-center space-x-3 mb-6">
                        <span class="w-10 h-10 rounded-xl bg-sky-100 text-sky-600 flex items-center justify-center text-lg">
                            <i class="fa-solid fa-water"></i>
                        </span>
                        <h3 class="text-xl sm:text-2xl font-bold text-slate-900">白天水上挑戰：與海龜攜手同行</h3>
                    </div>

                    <div class="space-y-6">
                        <div class="flex space-x-4">
                            <div class="flex-shrink-0 w-24 h-24 rounded-2xl overflow-hidden bg-slate-100">
                                <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?auto=format&fit=crop&w=300&q=80" alt="浮潛" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <h4 class="text-base sm:text-lg font-bold text-slate-800">生態浮潛 (Eco Snorkeling)</h4>
                                <p class="text-xs text-slate-500 mt-1 leading-relaxed">
                                    小琉球是全球綠蠵龜密集度最高的海域之一。跟著專業教練，在<strong>不驚擾、絕不觸碰</strong>的規範下，與溫柔巨龜在水中並肩同行。
                                </p>
                                <span class="inline-block mt-2 text-[10px] bg-sky-100 text-sky-700 font-semibold px-2 py-0.5 rounded">費用：約 NT$400 - 500 / 人</span>
                            </div>
                        </div>

                        <div class="flex space-x-4">
                            <div class="flex-shrink-0 w-24 h-24 rounded-2xl overflow-hidden bg-slate-100">
                                <img src="https://images.unsplash.com/photo-1517176118179-65244903d13c?auto=format&fit=crop&w=300&q=80" alt="SUP" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <h4 class="text-base sm:text-lg font-bold text-slate-800">SUP立槳 ＆ 透明獨木舟</h4>
                                <p class="text-xs text-slate-500 mt-1 leading-relaxed">
                                    近年最風靡的海上運動，推薦選擇夕陽黃昏場，悠閒站在立槳上，看著金黃夕陽染紅海面。透明獨木舟則讓您低下頭直接看見海龜游過！
                                </p>
                                <span class="inline-block mt-2 text-[10px] bg-emerald-100 text-emerald-700 font-semibold px-2 py-0.5 rounded">費用：約 NT$1,200 - 1,800 / 人</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Night Vibing -->
                <div class="bg-white rounded-3xl p-8 shadow-sm border border-slate-100/80">
                    <div class="flex items-center space-x-3 mb-6">
                        <span class="w-10 h-10 rounded-xl bg-amber-100 text-amber-600 flex items-center justify-center text-lg">
                            <i class="fa-solid fa-martini-glass-citrus"></i>
                        </span>
                        <h3 class="text-xl sm:text-2xl font-bold text-slate-900">暗夜夜生活：潮間帶與特色酒館</h3>
                    </div>

                    <div class="space-y-6">
                        <div class="flex space-x-4">
                            <div class="flex-shrink-0 w-24 h-24 rounded-2xl overflow-hidden bg-slate-100">
                                <img src="https://images.unsplash.com/photo-1529156069898-49953e39b3ac?auto=format&fit=crop&w=300&q=80" alt="酒吧" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <h4 class="text-base sm:text-lg font-bold text-slate-800">貳拾有陸 Bar / HighWave Bar</h4>
                                <p class="text-xs text-slate-500 mt-1 leading-relaxed">
                                    小島最具人氣的 Chill 酒吧。調酒師巧妙將小琉球在地元素融入微醺特調。在半開放式空間裡吹海風聽音樂，好不愜意。
                                </p>
                                <span class="inline-block mt-2 text-[10px] bg-amber-100 text-amber-700 font-semibold px-2 py-0.5 rounded">溫馨提醒：請勿酒駕 ｜ 開車不喝酒</span>
                            </div>
                        </div>

                        <div class="flex space-x-4">
                            <div class="flex-shrink-0 w-24 h-24 rounded-2xl overflow-hidden bg-slate-100">
                                <img src="https://images.unsplash.com/photo-1509198397868-475647b2a1e5?auto=format&fit=crop&w=300&q=80" alt="星空潮間帶" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <h4 class="text-base sm:text-lg font-bold text-slate-800">夜間生態導覽（潮間帶夜行）</h4>
                                <p class="text-xs text-slate-500 mt-1 leading-relaxed">
                                    打著手電筒跟著島民嚮導走。探訪礁岩縫中夜行性的奇怪海膽、發光貝類；在無光害林道尋找深夜盛開的魔幻之花「棋盤腳」。
                                </p>
                                <span class="inline-block mt-2 text-[10px] bg-slate-100 text-slate-700 font-semibold px-2 py-0.5 rounded">通常由民宿生態套票附贈</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Itinerary Schedule with Stars to save -->
    <section id="itinerary" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-slate-900 tracking-tight">黃金三日完美度假日程</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-500 mt-4 text-sm sm:text-base">無腦照著走，點擊行程右側的星號 <i class="fa-regular fa-star"></i>，即可動態將其打包至底部的「我的專屬手冊」，還能一鍵生成複製純文字與旅伴分享喔！</p>
            </div>

            <!-- Day Tabs -->
            <div class="flex flex-wrap justify-center gap-3 mb-10">
                <button onclick="switchDay(1)" id="day1Btn" class="day-tab px-5 py-3 rounded-2xl text-xs sm:text-sm font-bold bg-ocean-500 text-white shadow-md transition-all">DAY 1：登島與夕照微風</button>
                <button onclick="switchDay(2)" id="day2Btn" class="day-tab px-5 py-3 rounded-2xl text-xs sm:text-sm font-bold bg-slate-100 text-slate-600 hover:bg-slate-200 transition-all">DAY 2：海龜同游與潮汐</button>
                <button onclick="switchDay(3)" id="day3Btn" class="day-tab px-5 py-3 rounded-2xl text-xs sm:text-sm font-bold bg-slate-100 text-slate-600 hover:bg-slate-200 transition-all">DAY 3：晨曦破曉與歸航</button>
            </div>

            <!-- Timelines -->
            <div class="max-w-3xl mx-auto">
                <!-- Day 1 -->
                <div id="day1Content" class="day-content space-y-6">
                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-ocean-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-ocean-600 uppercase tracking-widest">10:30 - 11:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">順利登陸 & 快速取車</h4>
                                <p class="text-xs text-slate-500 mt-1">白沙港口下船。前往尚美租車行取車，騎行前往民宿放下行李、稍作休息。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY1-10:30 登陸取車')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-ocean-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-ocean-600 uppercase tracking-widest">12:00 - 13:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">午餐首享：柴燒「相思麵」</h4>
                                <p class="text-xs text-slate-500 mt-1">經典炭香肉燥相思麵加特製相思辣醬，美味開胃，揭開島民味覺序幕。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY1-12:00 午餐相思麵')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-ocean-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-ocean-600 uppercase tracking-widest">14:00 - 16:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">「花瓶岩」看海龜 ＆ 「美人洞」漫步</h4>
                                <p class="text-xs text-slate-500 mt-1">與最具地標代表性的「花瓶岩」合影，隨後漫步穿梭於美人洞嶙峋珊瑚礁崖之間。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY1-14:00 花瓶岩看海龜及美人洞')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-ocean-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-ocean-600 uppercase tracking-widest">17:00 - 18:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">「落日亭」海平線奢華落日</h4>
                                <p class="text-xs text-slate-500 mt-1">在遼闊的高台吹著溫熱海風，靜看整顆太陽沒入西方巴士海峽。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY1-17:00 落日亭觀看落日')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-ocean-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-ocean-600 uppercase tracking-widest">20:00 - Late</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">夜生活：酒吧極致微醺</h4>
                                <p class="text-xs text-slate-500 mt-1">走進半開放式的「貳拾有陸 Bar」，伴隨微涼夜風品嚐特製小島微醺。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY1-20:00 酒吧微醺之夜')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Day 2 -->
                <div id="day2Content" class="day-content space-y-6 hidden">
                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-emerald-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-emerald-600 uppercase tracking-widest">08:30 - 09:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">島民活力早餐：洪媽媽</h4>
                                <p class="text-xs text-slate-500 mt-1">早起品嚐極富在地特色的手工琉球粿、溫熱香甜賓士包，注入一整天的水上活力。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY2-08:30 洪媽媽早餐')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-emerald-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-emerald-600 uppercase tracking-widest">10:00 - 12:00</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">深潛 / 生態浮潛與海龜同游</h4>
                                <p class="text-xs text-slate-500 mt-1">重頭戲登場！在教練專業伴游與攝影下，在水晶般的果凍海中與巨大綠蠵龜夢幻共舞。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY2-10:00 浮潛與海龜共游')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-emerald-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-emerald-600 uppercase tracking-widest">14:00 - 16:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">網美老木拍大片 & 大福港踩水</h4>
                                <p class="text-xs text-slate-500 mt-1">在老木上迎浪留影，隨後去大福沙灘感受晶亮沙質與微涼海浪撫摸。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY2-14:00 網美老木拍照')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-emerald-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-emerald-600 uppercase tracking-widest">20:00 - 21:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">夜間生態探索：夜巡潮間帶</h4>
                                <p class="text-xs text-slate-500 mt-1">拿著電筒跟隨嚮導涉水。發覺沉睡的珊瑚礁生態與夜間綻放的棋盤腳魔幻之花。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY2-20:00 夜間生態導覽')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>
                </div>

                <!-- Day 3 -->
                <div id="day3Content" class="day-content space-y-6 hidden">
                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-amber-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-amber-600 uppercase tracking-widest">05:00 - 06:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">「旭日亭」金色曙光破曉</h4>
                                <p class="text-xs text-slate-500 mt-1">早起騎行直奔東側高地，看著萬道金光衝出波瀾海平線，逆著陽光許下願望。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY3-05:00 旭日亭看日出')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8 border-l-2 border-slate-200 pb-4">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-amber-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-amber-600 uppercase tracking-widest">09:30 - 11:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">避暑「山豬溝」與「厚石裙礁」透亮果凍海</h4>
                                <p class="text-xs text-slate-500 mt-1">躲進熱帶盤根錯節的山豬溝，隨後前往厚石裙礁間那座透亮無浪的果凍海天然泳池踩水。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY3-09:30 山豬溝與厚石裙礁')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>

                    <div class="relative pl-8">
                        <span class="absolute left-0 top-0 -translate-x-1/2 w-6 h-6 rounded-full bg-amber-500 border-4 border-white flex items-center justify-center text-[10px] text-white"></span>
                        <div class="flex justify-between items-start">
                            <div>
                                <span class="text-xs font-bold text-amber-600 uppercase tracking-widest">13:30 - 14:30</span>
                                <h4 class="text-base font-bold text-slate-900 mt-1">採購「麻花捲」伴手禮與不捨歸航</h4>
                                <p class="text-xs text-slate-500 mt-1">港口邊採買現搓脆香的手工麻花捲，歸還機車，帶著滿滿寶藍色回憶搭上回程快艇。</p>
                            </div>
                            <button onclick="toggleItinerary('DAY3-13:30 買麻花捲並搭船返港')" class="text-slate-300 hover:text-amber-500 transition-colors text-lg p-1"><i class="fa-solid fa-star"></i></button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Eco Promise Badge Generator & Budget Tool -->
    <section id="planner-tool" class="py-20 bg-slate-900 text-white relative">
        <div class="absolute inset-0 bg-[radial-gradient(circle_at_top_right,rgba(34,197,94,0.1),transparent_50%)]"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold tracking-tight">行前互動助手：預算估算 ＆ 生態認證</h2>
                <div class="h-1.5 w-16 bg-emerald-500 mx-auto mt-4 rounded-full"></div>
                <p class="text-slate-400 mt-4 text-sm sm:text-base">極致預算估算器可以幫助您秒算開銷；同時簽署永續宣言，客製並儲存您的數位「小琉球生態守護者」勳章證書！</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- Advanced Budget Calculator -->
                <div class="dark-glass rounded-3xl p-6 sm:p-8 border border-slate-800 shadow-xl flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-bold mb-6 flex items-center text-gradient"><i class="fa-solid fa-calculator mr-2 text-ocean-400"></i> 小島開銷精準預估器</h3>
                        
                        <div class="space-y-6">
                            <!-- People -->
                            <div>
                                <label class="block text-xs font-semibold text-slate-400 mb-2 uppercase tracking-wider">旅行總人數</label>
                                <div class="flex items-center space-x-3">
                                    <button onclick="updatePeople(-1)" class="w-10 h-10 rounded-xl bg-slate-800 hover:bg-slate-700 flex items-center justify-center font-bold text-lg transition-colors">-</button>
                                    <span id="calcPeople" class="text-lg font-extrabold text-white px-4">2</span>
                                    <button onclick="updatePeople(1)" class="w-10 h-10 rounded-xl bg-slate-800 hover:bg-slate-700 flex items-center justify-center font-bold text-lg transition-colors">+</button>
                                    <span class="text-xs text-slate-400">位旅伴</span>
                                </div>
                            </div>

                            <!-- Days -->
                            <div>
                                <label class="block text-xs font-semibold text-slate-400 mb-2 uppercase tracking-wider">探險天數</label>
                                <div class="grid grid-cols-3 gap-2">
                                    <button onclick="setCalcDays(1)" class="calc-day-btn px-2 py-2.5 rounded-xl text-xs font-bold bg-slate-800 text-slate-300 transition-all" id="btnCD1">1天 (當天往返)</button>
                                    <button onclick="setCalcDays(2)" class="calc-day-btn px-2 py-2.5 rounded-xl text-xs font-bold bg-slate-800 text-slate-300 transition-all" id="btnCD2">2天 1夜</button>
                                    <button onclick="setCalcDays(3)" class="calc-day-btn px-2 py-2.5 rounded-xl text-xs font-bold bg-ocean-500 text-white transition-all" id="btnCD3">3天 2夜</button>
                                </div>
                            </div>

                            <!-- New Accomodation Grade Selector -->
                            <div>
                                <label class="block text-xs font-semibold text-slate-400 mb-2 uppercase tracking-wider">民宿住宿檔次</label>
                                <select id="stayGrade" onchange="calcTotal()" class="w-full bg-slate-800 border border-slate-700 rounded-xl p-3 text-xs sm:text-sm text-white focus:outline-none focus:ring-2 focus:ring-ocean-500">
                                    <option value="1200">青年背包客棧 (約 NT$1,200 / 晚・人)</option>
                                    <option value="3200" selected>精緻文青設計民宿 (約 NT$3,200 / 晚・房)</option>
                                    <option value="4800">奢華 Villa 獨立水池房 (約 NT$4,800 / 晚・房)</option>
                                </select>
                            </div>

                            <!-- Custom item Checkbox packs -->
                            <div class="space-y-3">
                                <label class="block text-xs font-semibold text-slate-400 uppercase tracking-wider">自選活動項目</label>
                                
                                <label class="flex items-center space-x-3 bg-slate-800/40 p-3 rounded-xl cursor-pointer hover:bg-slate-800/80 transition-colors border border-slate-800">
                                    <input type="checkbox" id="itemFerry" checked onchange="calcTotal()" class="w-4 h-4 text-ocean-500 bg-slate-950 border-slate-700 rounded focus:ring-ocean-500">
                                    <div class="text-[11px] sm:text-xs">
                                        <p class="font-bold text-white">東港來回高速船票 (NT$410 / 人)</p>
                                        <p class="text-slate-400">往返台灣本島與小琉球客運船班</p>
                                    </div>
                                </label>

                                <label class="flex items-center space-x-3 bg-slate-800/40 p-3 rounded-xl cursor-pointer hover:bg-slate-800/80 transition-colors border border-slate-800">
                                    <input type="checkbox" id="itemScooter" checked onchange="calcTotal()" class="w-4 h-4 text-ocean-500 bg-slate-950 border-slate-700 rounded focus:ring-ocean-500">
                                    <div class="text-[11px] sm:text-xs">
                                        <p class="font-bold text-white">低碳電動機車租借 (NT$400 / 天，兩人一車)</p>
                                        <p class="text-slate-400">低碳靜音環島，暢行大斜坡必備</p>
                                    </div>
                                </label>

                                <label class="flex items-center space-x-3 bg-slate-800/40 p-3 rounded-xl cursor-pointer hover:bg-slate-800/80 transition-colors border border-slate-800">
                                    <input type="checkbox" id="itemWater" checked onchange="calcTotal()" class="w-4 h-4 text-ocean-500 bg-slate-950 border-slate-700 rounded focus:ring-ocean-500">
                                    <div class="text-[11px] sm:text-xs">
                                        <p class="font-bold text-white">生態浮潛 / SUP立槳水上行程 (NT$1,200 / 人)</p>
                                        <p class="text-slate-400">教練帶領不擾龜共游與專業水中拍照</p>
                                    </div>
                                </label>
                            </div>
                        </div>
                    </div>

                    <!-- Budget Total Output -->
                    <div class="bg-gradient-to-r from-ocean-950 to-slate-900 p-5 rounded-2xl border border-ocean-900/30 flex items-center justify-between mt-6">
                        <div>
                            <p class="text-xs text-slate-400">預估旅行總預算 (台幣)</p>
                            <p class="text-[10px] text-slate-500 mt-0.5">※ 含住宿、餐費、機車及上述自選</p>
                        </div>
                        <div class="text-right">
                            <span class="text-xl sm:text-3xl font-black text-transparent bg-clip-text bg-gradient-to-r from-ocean-400 to-emerald-400" id="totalPrice">NT$ 9,840</span>
                        </div>
                    </div>
                </div>

                <!-- Eco Guardian Certificate (New Interactive Interactive Feature) -->
                <div class="dark-glass rounded-3xl p-6 sm:p-8 border border-slate-800 shadow-xl flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-bold mb-2 flex items-center text-emerald-400"><i class="fa-solid fa-medal mr-2"></i> 守護蔚藍：生態承諾證書</h3>
                        <p class="text-slate-400 text-xs sm:text-sm mb-4">承諾保護綠蠵龜與珊瑚海洋生態。完成誓言即可生成並儲存您的客製證書：</p>
                        
                        <div class="space-y-2 bg-slate-950/60 p-4 rounded-2xl border border-slate-850 text-xs text-slate-300 mb-4">
                            <label class="flex items-center space-x-2.5 cursor-pointer">
                                <input type="checkbox" id="pledge1" class="w-3.5 h-3.5 text-emerald-500 bg-slate-900 border-slate-700 rounded focus:ring-emerald-500">
                                <span>與海龜游泳時保持 5 公尺安全距離，<strong>絕不觸摸</strong>或驚擾牠們。</span>
                            </label>
                            <label class="flex items-center space-x-2.5 cursor-pointer">
                                <input type="checkbox" id="pledge2" class="w-3.5 h-3.5 text-emerald-500 bg-slate-900 border-slate-700 rounded focus:ring-emerald-500">
                                <span>下水遊玩前，僅使用<strong>海洋友善防曬乳</strong>或穿著物理防曬水母衣。</span>
                            </label>
                            <label class="flex items-center space-x-2.5 cursor-pointer">
                                <input type="checkbox" id="pledge3" class="w-3.5 h-3.5 text-emerald-500 bg-slate-900 border-slate-700 rounded focus:ring-emerald-500">
                                <span>攜帶個人環保水壺，踐行島上「減塑減廢」低碳度假承諾。</span>
                            </label>
                        </div>

                        <!-- Name field -->
                        <div class="flex space-x-2 mb-4">
                            <input type="text" id="guardianName" placeholder="請輸入證書上的守護者名字..." class="flex-1 bg-slate-800 border border-slate-700 rounded-xl px-4 py-2 text-xs sm:text-sm text-white focus:outline-none focus:ring-2 focus:ring-emerald-500">
                            <button onclick="generateEcoBadge()" class="bg-emerald-500 hover:bg-emerald-600 text-white text-xs sm:text-sm font-bold px-4 py-2 rounded-xl transition-colors">生成證書</button>
                        </div>

                        <!-- Badge Render Box -->
                        <div id="badgePreviewContainer" class="hidden relative bg-slate-50 text-slate-800 p-5 rounded-2xl border border-slate-200 text-center shadow-lg transition-all duration-300 transform scale-95 opacity-0">
                            <!-- Background soft watermark of a sea turtle -->
                            <div class="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1544551763-46a013bb70d5?auto=format&fit=crop&w=400&q=80')] bg-cover bg-center opacity-[0.04] rounded-2xl pointer-events-none"></div>
                            
                            <div class="border-2 border-dashed border-emerald-500/40 p-4 rounded-xl relative z-10">
                                <span class="text-2xl text-emerald-500"><i class="fa-solid fa-certificate"></i></span>
                                <h4 class="text-sm font-black tracking-widest text-slate-900 mt-1 uppercase">小琉球生態護航證書</h4>
                                <p class="text-[9px] text-slate-400 mt-0.5">ECO-GUARDIAN OF LAMBAI ISLAND</p>
                                
                                <p class="text-xs text-slate-700 mt-4 px-2 italic font-serif">
                                    特此感謝 <strong class="text-emerald-600 underline font-sans" id="renderName">潛水員</strong> 承諾守護珊瑚礁與綠蠵龜群落，踐行低碳永續島嶼度假誓言。
                                </p>
                                
                                <div class="flex justify-between items-center text-[8px] text-slate-400 mt-6 pt-3 border-t border-slate-100">
                                    <span>認證時間：2026年夏季</span>
                                    <span class="bg-emerald-50 text-emerald-700 font-bold px-2 py-0.5 rounded-full border border-emerald-100">Lambai Ocean Guard</span>
                                </div>
                            </div>
                            <button onclick="saveBadgeAsText()" class="mt-3 w-full bg-slate-800 hover:bg-slate-700 text-white font-bold py-1.5 rounded-xl text-[10px] transition-colors">
                                <i class="fa-solid fa-copy mr-1"></i> 複製證書認證碼分享
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Checklist & Customized Itinerary Hand-book -->
    <section class="py-20 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- Checklist -->
                <div class="bg-white rounded-3xl p-6 sm:p-8 border border-slate-100 shadow-sm flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-bold text-slate-900 mb-2 flex items-center"><i class="fa-solid fa-clipboard-list mr-2 text-emerald-500"></i> 小島行囊必備 Checklist</h3>
                        <p class="text-slate-500 text-xs sm:text-sm mb-6">點擊核對您已打包好的行囊，輕裝上陣，確保萬無一失：</p>
                        
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-3" id="checklistContainer">
                            <!-- Populated dynamically by JS -->
                        </div>
                    </div>
                </div>

                <!-- Star Pack Custom Itinerary -->
                <div class="bg-white rounded-3xl p-6 sm:p-8 border border-slate-100 shadow-sm flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-bold text-slate-900 mb-2 flex items-center justify-between">
                            <span><i class="fa-solid fa-star mr-1 text-amber-500"></i> 我的專屬收藏手冊</span>
                            <button onclick="clearCustomItinerary()" class="text-xs text-slate-400 hover:text-red-500 transition-colors">全部清空</button>
                        </h3>
                        <p class="text-slate-500 text-xs sm:text-sm mb-6">點選上方三日日程項目右側的星號 <i class="fa-regular fa-star"></i>，即可在這裡打包您的特製行程：</p>
                        
                        <div id="customItineraryList" class="space-y-2 text-xs sm:text-sm text-slate-400">
                            <!-- Dynamically loaded -->
                            <p class="text-center py-8">目前您的手冊還是空的。快點選上方三日日程項目旁的星號 <i class="fa-regular fa-star"></i> 把它們裝進來吧！</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ & Marine Preservation Accordion -->
    <section class="py-20 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6">
            <div class="text-center mb-16">
                <span class="bg-emerald-100 text-emerald-800 text-xs font-bold px-3 py-1 rounded-full">遊島Q&A</span>
                <h2 class="text-3xl font-bold text-slate-900 mt-2">常見旅遊與海洋守護提問</h2>
                <div class="h-1.5 w-16 bg-ocean-500 mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="space-y-4">
                <div class="bg-slate-50 p-6 rounded-2xl border border-slate-100">
                    <h4 class="font-bold text-slate-900 text-sm sm:text-base mb-2"><i class="fa-solid fa-circle-question mr-2 text-emerald-500"></i>1. 看到海龜可以跟牠拍照或觸碰嗎？有什麼罰則嗎？</h4>
                    <p class="text-xs sm:text-sm text-slate-500 leading-relaxed">
                        <strong>絕對不可碰觸、追逐或阻擋海龜！</strong>綠蠵龜在台灣屬於受法律嚴格保護的保育類動物。若被錄影檢舉有觸碰海龜之行為，將面臨<strong>最高 NT$6萬 至 30萬元台幣</strong> 的天價罰款！請務必與海龜保持「至少 5 公尺（兩隻手臂長）」以上安全距離。
                    </p>
                </div>

                <div class="bg-slate-50 p-6 rounded-2xl border border-slate-100">
                    <h4 class="font-bold text-slate-900 text-sm sm:text-base mb-2"><i class="fa-solid fa-circle-question mr-2 text-ocean-500"></i>2. 什麼季節最適合去小琉球？冬天可以玩水浮潛嗎？</h4>
                    <p class="text-xs sm:text-sm text-slate-500 leading-relaxed">
                        小琉球是台灣唯一的珊瑚礁海島，受台灣本島東北季風與寒流影響極小。一年四季平均水溫都在 25°C 左右。即使是冬天（11月 ~ 隔年3月），小琉球依然溫暖晴朗，是非常棒的「避冬避寒」浮潛共游天堂。
                    </p>
                </div>

                <div class="bg-slate-50 p-6 rounded-2xl border border-slate-100">
                    <h4 class="font-bold text-slate-900 text-sm sm:text-base mb-2"><i class="fa-solid fa-circle-question mr-2 text-pink-500"></i>3. 搭船會很容易暈船嗎？應該如何有效預防？</h4>
                    <p class="text-xs sm:text-sm text-slate-500 leading-relaxed">
                        東港到小琉球船程僅約 25-30 分鐘，如果遇到風浪大，建議在<strong>開船前 30 分鐘</strong>提前服用暈船藥。在船艙內，建議<strong>坐在靠船尾、靠窗戶</strong>的位置（船尾震盪起伏幅度最小），闭目養神可大幅減緩不適。
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- GitHub Pages Deployment Guide Widget (Specially tailored for User) -->
    <section class="py-12 bg-slate-950 text-white relative border-t border-slate-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6">
            <div class="bg-slate-900/60 rounded-3xl p-6 sm:p-8 border border-slate-800">
                <div class="flex items-center space-x-3 mb-4 cursor-pointer" onclick="toggleGithubGuide()">
                    <span class="text-3xl text-sky-400"><i class="fa-brands fa-github"></i></span>
                    <div class="flex-1">
                        <h3 class="text-base sm:text-lg font-bold">🛠️ 3分鐘如何將本指南部署到 GitHub Pages？</h3>
                        <p class="text-xs text-slate-400 mt-0.5">點選此欄展開/收合極簡部署教學步驟</p>
                    </div>
                    <span id="githubToggleIcon" class="text-slate-400 text-lg transition-transform duration-300 transform"><i class="fa-solid fa-chevron-down"></i></span>
                </div>

                <div id="githubGuideContent" class="hidden mt-6 pt-6 border-t border-slate-800 text-xs sm:text-sm text-slate-300 space-y-4">
                    <p>當您取得本網頁的完整代碼後，請按照以下步驟部署，即可免費獲得專屬觀光網址：</p>
                    <ol class="list-decimal list-inside space-y-2.5 text-slate-400">
                        <li>註冊並登入您的 <a href="https://github.com" target="_blank" class="text-sky-400 underline hover:text-sky-300">GitHub 帳號</a>。</li>
                        <li>創建一個全新的 Repository (代碼庫)，命名為 <code class="bg-slate-800 text-slate-200 px-1.5 py-0.5 rounded text-xs">liuqiu-guide</code>。</li>
                        <li>在此 Repository 中新建一個文件，命名為 <strong class="text-white">index.html</strong>。</li>
                        <li>將右側編輯器中的完整 HTML 原始碼複製並粘貼到該文件中，保存並 Commit。</li>
                        <li>前往 Repository 的 <strong class="text-white">Settings</strong> &rarr; <strong class="text-white">Pages</strong>。</li>
                        <li>在 Build and deployment 區塊將 Branch 選擇為 <code class="bg-slate-800 text-slate-250 px-1.5 py-0.5 rounded">main</code> (或master)，點選 <strong class="text-sky-400">Save</strong> 保存。</li>
                        <li>稍等 1-2 分鐘重新整理，GitHub 就會自動生成一個類似 <code class="bg-slate-800 text-emerald-400 px-1.5 py-0.5 rounded text-xs">https://你的帳號.github.io/liuqiu-guide/</code> 的專屬綠色安全連結囉！</li>
                    </ol>
                    <div class="p-3 bg-slate-800/50 rounded-xl border border-slate-700 flex items-center space-x-2 text-xs">
                        <span class="text-emerald-400"><i class="fa-solid fa-circle-check"></i></span>
                        <p class="text-slate-300">本 HTML 代碼已自備所有前端 UI 資源、Tailwind 與 FontAwesome，無需安裝任何 node.js 依賴，真正開箱即部署！</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-950 text-slate-500 py-12 border-t border-slate-900 text-center sm:text-left">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col sm:flex-row justify-between items-center space-y-6 sm:space-y-0">
                <div>
                    <div class="flex items-center space-x-2 justify-center sm:justify-start">
                        <span class="w-8 h-8 bg-ocean-500 rounded-lg flex items-center justify-center text-white font-black shadow-md shadow-ocean-500/20">L</span>
                        <span class="text-base font-bold text-white tracking-widest font-sans">藍海織夢 ｜ 小琉球度假指南</span>
                    </div>
                    <p class="text-xs text-slate-600 mt-2">© 2026 Lambai Island Guide. 響應式低碳海島觀光官網 ｜ 完美適配 GitHub Pages 靜態託管。</p>
                </div>
                
                <div class="flex space-x-4 text-xs">
                    <button onclick="showToast('🍃 生態守護是我們最珍貴的資產，感謝一同愛惜綠蠵龜！')" class="hover:text-emerald-400 transition-colors"><i class="fa-solid fa-leaf text-base mr-1"></i> 生態永續</button>
                    <span class="text-slate-800">|</span>
                    <button onclick="showToast('🐢 綠色和平、海洋保育，低碳小島永垂不朽')" class="hover:text-white transition-colors"><i class="fa-solid fa-heart text-base mr-1"></i> 保育合作</button>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Core Webpack-less Vanilla JS to power UI state seamlessly

        // 1. Sticky & Color-Changing Navbar on Scroll
        const mainNav = document.getElementById('mainNav');
        const navLogoText = document.getElementById('navLogoText');
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 80) {
                mainNav.classList.remove('bg-transparent');
                mainNav.classList.add('bg-white', 'shadow-md', 'h-16');
                mainNav.classList.remove('h-20');
                navLogoText.classList.remove('text-white');
                navLogoText.classList.add('text-slate-800');
                
                // Adjust desktop menu color links
                const links = mainNav.querySelectorAll('a:not(.bg-ocean-500)');
                links.forEach(link => {
                    link.classList.remove('text-white', 'hover:text-ocean-200');
                    link.classList.add('text-slate-600', 'hover:text-ocean-600');
                });
            } else {
                mainNav.classList.add('bg-transparent');
                mainNav.classList.remove('bg-white', 'shadow-md', 'h-16');
                mainNav.classList.add('h-20');
                navLogoText.classList.add('text-white');
                navLogoText.classList.remove('text-slate-800');
                
                const links = mainNav.querySelectorAll('a:not(.bg-ocean-500)');
                links.forEach(link => {
                    link.classList.add('text-white', 'hover:text-ocean-200');
                    link.classList.remove('text-slate-600', 'hover:text-ocean-600');
                });
            }
        });

        // 2. Mobile Drawer Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mobileDrawer = document.getElementById('mobileDrawer');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileDrawer.classList.toggle('hidden');
        });

        function closeDrawer() {
            mobileDrawer.classList.add('hidden');
        }

        // Smooth scroll helper
        function scrollToId(id) {
            const el = document.getElementById(id);
            if (el) {
                el.scrollIntoView({ behavior: 'smooth' });
                closeDrawer();
            }
        }

        // 3. Custom Toast Notification System
        function showToast(message, isInfo = true) {
            const toastBox = document.getElementById('toastBox');
            const toastMsg = document.getElementById('toastMsg');
            const toastIcon = document.getElementById('toastIcon');
            
            toastMsg.innerText = message;
            if (isInfo) {
                toastIcon.innerHTML = `<i class="fa-solid fa-circle-check"></i>`;
                toastIcon.className = "text-emerald-400 text-xl";
            } else {
                toastIcon.innerHTML = `<i class="fa-solid fa-triangle-exclamation"></i>`;
                toastIcon.className = "text-sunset-500 text-xl";
            }
            
            toastBox.classList.remove('translate-y-20', 'opacity-0');
            toastBox.classList.add('translate-y-0', 'opacity-100');
            
            setTimeout(() => {
                toastBox.classList.remove('translate-y-0', 'opacity-100');
                toastBox.classList.add('translate-y-20', 'opacity-0');
            }, 3000);
        }

        // 4. Attractions Filter Logic (Added explicit event parameter to fix strict mode exceptions)
        function filterSpots(category, event) {
            const cards = document.querySelectorAll('.spot-card');
            const btns = document.querySelectorAll('.spot-filter-btn');
            
            btns.forEach(btn => {
                btn.className = "spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-white text-slate-600 hover:bg-slate-100 transition-all shadow-sm border border-slate-200";
            });
            
            if (event && event.currentTarget) {
                event.currentTarget.className = "spot-filter-btn px-4 py-2 rounded-full text-xs sm:text-sm font-semibold bg-ocean-500 text-white shadow-md transition-all";
            }

            cards.forEach(card => {
                if (category === 'all' || card.getAttribute('data-category') === category) {
                    card.classList.remove('hidden');
                    card.classList.add('block');
                } else {
                    card.classList.remove('block');
                    card.classList.add('hidden');
                }
            });
        }

        // 5. Day-by-Day Itinerary Tab Switcher
        function switchDay(dayNum) {
            const days = [1, 2, 3];
            days.forEach(num => {
                const btn = document.getElementById(`day${num}Btn`);
                const content = document.getElementById(`day${num}Content`);
                
                if (num === dayNum) {
                    btn.className = "day-tab px-5 py-3 rounded-2xl text-xs sm:text-sm font-bold bg-ocean-500 text-white shadow-md transition-all";
                    content.classList.remove('hidden');
                } else {
                    btn.className = "day-tab px-5 py-3 rounded-2xl text-xs sm:text-sm font-bold bg-slate-100 text-slate-600 hover:bg-slate-200 transition-all";
                    content.classList.add('hidden');
                }
            });
        }

        // 6. Interactive Custom Itinerary Builder
        let savedItinerary = [];
        function toggleItinerary(itemName) {
            const index = savedItinerary.indexOf(itemName);
            if (index > -1) {
                savedItinerary.splice(index, 1);
                showToast(`已從我的手冊移出：${itemName}`, false);
            } else {
                savedItinerary.push(itemName);
                showToast(`已成功打包加入手冊！⭐️`);
            }
            renderSavedItinerary();
        }

        function clearCustomItinerary() {
            savedItinerary = [];
            renderSavedItinerary();
            showToast('已清空您的自製手冊。', false);
        }

        function renderSavedItinerary() {
            const listContainer = document.getElementById('customItineraryList');
            if (savedItinerary.length === 0) {
                listContainer.innerHTML = `<p class="text-center py-8">目前您的手冊還是空的。快點選上方三日日程項目旁的星號 <i class="fa-regular fa-star"></i> 把它們裝進來吧！</p>`;
                return;
            }

            let html = '<ul class="space-y-2 bg-slate-50 p-4 rounded-2xl border border-slate-100">';
            savedItinerary.forEach((item, index) => {
                html += `
                    <li class="flex items-center justify-between py-1.5 border-b border-slate-100 last:border-0 text-slate-700 text-xs">
                        <span><i class="fa-solid fa-circle-check text-emerald-500 mr-2"></i> ${item}</span>
                        <button onclick="toggleItinerary('${item}')" class="text-slate-400 hover:text-red-500 transition-colors"><i class="fa-solid fa-trash-can"></i></button>
                    </li>
                `;
            });
            html += `
                <div class="mt-4 pt-3 border-t border-slate-100 text-center">
                    <button onclick="shareItinerary()" class="w-full bg-ocean-500 hover:bg-ocean-600 text-white font-bold py-2 px-3 rounded-xl text-xs transition-colors shadow">
                        <i class="fa-solid fa-share-nodes mr-1"></i> 複製我的特製行程純文字
                    </button>
                </div>
            `;
            html += '</ul>';
            listContainer.innerHTML = html;
        }

        function shareItinerary() {
            const textToCopy = `我的小琉球客製化夢幻探險行程：\n` + savedItinerary.map((it, idx) => `[步驟 ${idx+1}] ${it}`).join('\n') + `\n\n— 本指南生成自「藍海織夢 ｜ 小琉球極致蔚藍指南」`;
            
            // Fallback for copying text within iframes
            const textarea = document.createElement("textarea");
            textarea.value = textToCopy;
            document.body.appendChild(textarea);
            textarea.select();
            try {
                document.execCommand('copy');
                showToast("🎉 行程純文字複製成功！快快去貼給您的旅伴吧！");
            } catch (err) {
                showToast("複製失敗，請手動框選文字複製", false);
            }
            document.body.removeChild(textarea);
        }

        // 7. Interactive Map Spot Details
        function showMapPin(title, desc) {
            const titleEl = document.getElementById('mapInfoText');
            const panelEl = document.getElementById('mapDetailPanel');
            
            titleEl.innerHTML = `<span class="bg-ocean-500/15 px-3 py-1 rounded-full text-white border border-ocean-500/35 font-bold">${title}</span>`;
            panelEl.innerHTML = `<span class="text-white font-medium text-xs leading-relaxed">${desc}</span>`;
            
            showToast(`已虛擬環島至：${title}`);
        }

        // 8. Advanced Budget Calculator State
        let calcPeople = 2;
        let calcDays = 3;

        function updatePeople(change) {
            calcPeople += change;
            if (calcPeople < 1) calcPeople = 1;
            document.getElementById('calcPeople').innerText = calcPeople;
            calcTotal();
        }

        function setCalcDays(days) {
            calcDays = days;
            const buttons = document.querySelectorAll('.calc-day-btn');
            buttons.forEach(btn => {
                btn.className = "calc-day-btn px-2 py-2.5 rounded-xl text-xs font-bold bg-slate-800 text-slate-300 transition-all";
            });
            document.getElementById(`btnCD${days}`).className = "calc-day-btn px-2 py-2.5 rounded-xl text-xs font-bold bg-ocean-500 text-white transition-all";
            calcTotal();
        }

        function calcTotal() {
            let stayCostPerNight = parseFloat(document.getElementById('stayGrade').value);
            let basicFoodCostPerDay = 500; // Average cost of food
            
            let total = 0;
            
            // 1. Ferry ticket
            if (document.getElementById('itemFerry').checked) {
                total += 410 * calcPeople;
            }
            // 2. Scooter (1 scooter for every 2 people)
            if (document.getElementById('itemScooter').checked) {
                let scooterCount = Math.ceil(calcPeople / 2);
                total += scooterCount * 400 * calcDays;
            }
            // 3. Water Activity
            if (document.getElementById('itemWater').checked) {
                total += 1200 * calcPeople;
            }

            // 4. Accommodation
            let nights = calcDays - 1;
            if (nights < 0) nights = 0;
            
            if (nights > 0) {
                if (document.getElementById('stayGrade').value == "1200") {
                    // Backpacker rate is per-person
                    total += stayCostPerNight * calcPeople * nights;
                } else {
                    // Room rate is per-room (approx 2 people per room)
                    let roomCount = Math.ceil(calcPeople / 2);
                    total += roomCount * stayCostPerNight * nights;
                }
            }

            // 5. Food cost
            total += basicFoodCostPerDay * calcDays * calcPeople;

            document.getElementById('totalPrice').innerText = `NT$ ${total.toLocaleString()}`;
        }

        // 9. Eco Badge Generator
        function generateEcoBadge() {
            const p1 = document.getElementById('pledge1').checked;
            const p2 = document.getElementById('pledge2').checked;
            const p3 = document.getElementById('pledge3').checked;
            const name = document.getElementById('guardianName').value.trim();

            if (!p1 || !p2 || !p3) {
                showToast("請先勾選閱讀並承諾上述三條保護海龜的誓言喔！", false);
                return;
            }
            if (name === "") {
                showToast("請輸入守護者姓名以供證書認證！", false);
                return;
            }

            document.getElementById('renderName').innerText = name;
            const previewBox = document.getElementById('badgePreviewContainer');
            
            previewBox.classList.remove('hidden');
            setTimeout(() => {
                previewBox.classList.remove('scale-95', 'opacity-0');
                previewBox.classList.add('scale-100', 'opacity-100');
            }, 50);

            showToast("🎉 生態證書生成成功！感謝您守護小島生態環境！");
        }

        function saveBadgeAsText() {
            const name = document.getElementById('renderName').innerText;
            const randCode = "ECO-" + Math.floor(Math.random() * 900000 + 100000);
            const text = `【小琉球生態護航證書】\n護航者：${name}\n認證編碼：${randCode}\n認證時間：2026年夏季\n\n「海洋友善，減塑旅行。我已加入綠蠵龜守護聯盟！」`;
            
            const textarea = document.createElement("textarea");
            textarea.value = text;
            document.body.appendChild(textarea);
            textarea.select();
            try {
                document.execCommand('copy');
                showToast("🎉 證書認證純文字複製成功！快拿去社群動態分享吧！");
            } catch (err) {
                showToast("複製失敗，請手動框選文字", false);
            }
            document.body.removeChild(textarea);
        }

        // 10. Packing List Items
        const packingItems = [
            { text: "機車駕照 (租車必查！)" },
            { text: "身分證 / 健保卡" },
            { text: "海洋友善防曬乳" },
            { text: "個人泳衣 / 水母衣" },
            { text: "防滑厚底涼鞋 / 拖鞋" },
            { text: "手機防水袋" },
            { text: "個人隨行環保水壺" },
            { text: "暈船藥 (搭船前30分吃)" }
        ];

        function renderChecklist() {
            const container = document.getElementById('checklistContainer');
            container.innerHTML = "";
            
            packingItems.forEach((item, index) => {
                const itemDiv = document.createElement('div');
                itemDiv.className = "flex items-center space-x-3 bg-slate-50 p-3.5 rounded-2xl hover:bg-slate-100 transition-colors cursor-pointer border border-slate-100";
                itemDiv.innerHTML = `
                    <input type="checkbox" id="pack-${index}" class="w-4 h-4 text-emerald-500 bg-white border-slate-300 rounded focus:ring-emerald-500 cursor-pointer">
                    <label for="pack-${index}" class="text-xs sm:text-sm text-slate-700 font-medium cursor-pointer select-none">${item.text}</label>
                `;
                container.appendChild(itemDiv);
            });
        }

        // 11. GitHub Pages Expandable Widget Handler
        function toggleGithubGuide() {
            const content = document.getElementById('githubGuideContent');
            const icon = document.getElementById('githubToggleIcon');
            
            content.classList.toggle('hidden');
            if (content.classList.contains('hidden')) {
                icon.className = "text-slate-400 text-lg transition-transform duration-300 transform rotate-0";
            } else {
                icon.className = "text-slate-400 text-lg transition-transform duration-300 transform rotate-180";
            }
        }

        // Initialize App State
        window.onload = function() {
            calcTotal();
            renderChecklist();
            
            // Randomly simulate current Tide level on refresh for a fun experience
            const tides = [
                { text: "乾潮 (低潮期)", sub: "厚石果凍海、潮間帶步道的黃金探秘期！" },
                { text: "滿潮 (高潮期)", sub: "海水極滿，美人洞、花瓶岩浮潛看巨龜好時機！" },
                { text: "退潮中", sub: "潮水正退去，準備前往大福漁港看老木的最佳探路時機。" }
            ];
            const chosen = tides[Math.floor(Math.random() * tides.length)];
            document.getElementById('tideText').innerText = chosen.text;
            document.getElementById('tideSubText').innerText = chosen.sub;

            // Welcome greeting toast
            setTimeout(() => {
                showToast("🌊 準備好跟巨龜並肩同行嗎？開啟您的蔚藍島嶼旅程！");
            }, 1000);
        };
    </script>
</body>
</html>
