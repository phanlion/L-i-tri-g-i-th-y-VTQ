<!DOCTYPE html>
<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tri Ân Thầy Vũ Tá Quyền — Gửi Từ Phan Hòa Phát</title>
    <!-- Google Fonts: Playfair Display for Luxury, Montserrat for Modern Body -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,600;0,700;1,400&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Font Awesome for beautiful luxury icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- GSAP for Cinematic Animations -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        serif: ['Playfair Display', 'serif'],
                        sans: ['Montserrat', 'sans-serif'],
                    },
                    colors: {
                        luxuryRed: {
                            light: '#ff2d55',
                            DEFAULT: '#900d0d',
                            dark: '#4a0000',
                            glow: '#ff1a1a'
                        },
                        luxuryDark: {
                            DEFAULT: '#0a0505',
                            card: '#160a0a'
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* */
        body {
            background-color: #050202;
            color: #f5f0f0;
            overflow-x: hidden;
        }

        @media (min-width: 1025px) {
            body {
                cursor: none; /* Chỉ ẩn con trỏ chuột trên máy tính để tránh lỗi thiết bị di động */
            }
        }

        /* Hiệu ứng kính bóng bẩy (Luxury Glassmorphism) */
        .luxury-glass {
            background: rgba(22, 10, 10, 0.45);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 45, 85, 0.15);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.6);
            transition: all 0.5s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .luxury-glass:hover {
            border-color: rgba(255, 26, 26, 0.45);
            box-shadow: 0 0 30px rgba(255, 26, 26, 0.2);
            transform: translateY(-2px);
        }

        /* Định dạng Custom Cursor */
        .custom-cursor-dot {
            width: 8px;
            height: 8px;
            background-color: #ff2d55;
            position: fixed;
            border-radius: 50%;
            pointer-events: none;
            z-index: 9999;
            transform: translate(-50%, -50%);
            transition: width 0.15s, height 0.15s, opacity 0.3s;
            opacity: 0;
        }

        .custom-cursor-outline {
            width: 40px;
            height: 40px;
            border: 1px solid rgba(255, 45, 85, 0.5);
            position: fixed;
            border-radius: 50%;
            pointer-events: none;
            z-index: 9998;
            transform: translate(-50%, -50%);
            transition: transform 0.1s cubic-bezier(0.175, 0.885, 0.32, 1.275), border-color 0.2s, background-color 0.2s, opacity 0.3s;
            opacity: 0;
        }

        /* Hiệu ứng chữ phát sáng */
        .glow-text-red {
            text-shadow: 0 0 10px rgba(255, 26, 26, 0.6), 0 0 30px rgba(255, 26, 26, 0.3);
        }

        .glow-border-red {
            box-shadow: inset 0 0 15px rgba(255, 26, 26, 0.2), 0 0 15px rgba(255, 26, 26, 0.2);
        }

        /* Các khối hào quang mờ ảo ở nền (Ambient Orbs) */
        .ambient-orb {
            position: absolute;
            width: 45vw;
            height: 45vw;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(144, 13, 13, 0.25) 0%, rgba(5, 2, 2, 0) 70%);
            filter: blur(50px);
            pointer-events: none;
            z-index: 0;
        }

        /* Thanh tiến trình cuộn trang */
        #scroll-progress {
            position: fixed;
            top: 0;
            left: 0;
            height: 3px;
            background: linear-gradient(to right, #900d0d, #ff2d55, #ff6b6b);
            z-index: 10000;
            width: 0%;
        }

        /* Chuyển động lơ lửng vật lý */
        @keyframes physics-float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-12px) rotate(3deg); }
        }
        .physics-float {
            animation: physics-float 6s ease-in-out infinite;
        }

        /* Trái tim và biểu thức vật lý bay lên khi nhấp chuột */
        .floating-heart-emoji {
            position: absolute;
            pointer-events: none;
            animation: floatUpAndFade 1.2s cubic-bezier(0.16, 1, 0.3, 1) forwards;
            font-size: 1.5rem;
            z-index: 30;
        }

        @keyframes floatUpAndFade {
            0% {
                transform: translateY(0) scale(0.5);
                opacity: 1;
            }
            100% {
                transform: translateY(-120px) translateX(var(--random-x, 20px)) scale(1.2) rotate(var(--random-rotate, 15deg));
                opacity: 0;
            }
        }

        /* Tắt Custom Cursor trên các thiết bị cảm ứng để tránh lỗi UI */
        @media (max-width: 1024px) {
            .custom-cursor-dot, .custom-cursor-outline {
                display: none !important;
            }
        }
    </style>
</head>
<body class="selection:bg-luxuryRed selection:text-white relative">

    <!-- -->
    <!-- Scroll Progress Indicator -->
    <div id="scroll-progress"></div>

    <!-- Custom Cursor Elements -->
    <div class="custom-cursor-dot" id="cursor-dot"></div>
    <div class="custom-cursor-outline" id="cursor-outline"></div>

    <!-- Canvas sinh các hạt bụi sáng chuyển động ngẫu nhiên trên toàn trang -->
    <canvas id="particles-canvas" class="fixed top-0 left-0 w-full h-full pointer-events-none z-10 opacity-70"></canvas>

    <!-- Header / Thanh điều hướng -->
    <header class="fixed top-0 left-0 w-full z-50 transition-all duration-500 py-5 px-6 md:px-12">
        <nav class="max-w-7xl mx-auto flex justify-between items-center luxury-glass px-6 py-3.5 rounded-full border border-luxuryRed/10">
            <a href="#hero" class="font-serif text-lg md:text-xl font-bold tracking-widest text-white hover:text-luxuryRed-light transition duration-300">
                W.T.Q <span class="text-xs text-luxuryRed-light font-sans font-normal tracking-normal ml-1">PHYSICS</span>
            </a>
            <div class="hidden md:flex items-center space-x-8 text-sm uppercase tracking-wider font-semibold">
                <a href="#intro" class="hover:text-luxuryRed-light transition duration-300">Người Thầy</a>
                <a href="#gratitude" class="hover:text-luxuryRed-light transition duration-300">Lời Cảm Ơn</a>
                <a href="#timeline" class="hover:text-luxuryRed-light transition duration-300">Thanh Xuân</a>
                <a href="#wishes" class="hover:text-luxuryRed-light transition duration-300">Lời Chúc</a>
            </div>
            <div>
                <a href="#wishes" class="bg-gradient-to-r from-luxuryRed to-luxuryRed-light text-white text-xs md:text-sm font-semibold px-5 py-2.5 rounded-full uppercase tracking-wider transition-all duration-300 hover:shadow-[0_0_15px_rgba(255,45,85,0.6)] transform hover:-translate-y-0.5">
                    Gửi Lòng Biết Ơn
                </a>
            </div>
        </nav>
    </header>

    <!-- Ambient Background Lighting Orbs -->
    <div class="ambient-orb top-[-10%] left-[-10%]"></div>
    <div class="ambient-orb top-[40%] right-[-15%]"></div>
    <div class="ambient-orb bottom-[10%] left-[-10%]"></div>

    <!-- -->
    <!-- 1. HERO SECTION -->
    <section id="hero" class="relative min-h-screen flex items-center justify-center pt-24 overflow-hidden z-20">
        <!-- Spacetime coordinate warp lines (Mô phỏng không-thời gian bẻ cong của Thuyết tương đối rộng) -->
        <div class="absolute inset-0 opacity-15 pointer-events-none flex items-center justify-center">
            <svg class="w-full h-full max-w-7xl" viewBox="0 0 1000 1000" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M 0,500 Q 250,450 500,500 T 1000,500" stroke="#ff2d55" stroke-width="1.5" />
                <path d="M 0,400 Q 250,300 500,500 T 1000,600" stroke="#ff2d55" stroke-width="0.75" />
                <path d="M 0,600 Q 250,700 500,500 T 1000,400" stroke="#ff2d55" stroke-width="0.75" />
                <path d="M 500,0 Q 450,250 500,500 T 500,1000" stroke="#ff2d55" stroke-width="1.5" />
                <path d="M 400,0 Q 300,250 500,500 T 600,1000" stroke="#ff2d55" stroke-width="0.75" />
                <path d="M 600,0 Q 700,250 500,500 T 400,1000" stroke="#ff2d55" stroke-width="0.75" />
                <circle cx="500" cy="500" r="150" stroke="#ff2d55" stroke-width="1" stroke-dasharray="8 8" />
                <circle cx="500" cy="500" r="300" stroke="#ff2d55" stroke-width="0.5" />
            </svg>
        </div>

        <!-- Ambient lighting behind titles -->
        <div class="absolute w-[500px] h-[500px] bg-luxuryRed/10 rounded-full blur-[120px] top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 pointer-events-none"></div>

        <div class="max-w-5xl mx-auto text-center px-4 z-10 flex flex-col items-center">
            <!-- Animated physics-like icon badge -->
            <div class="mb-6 opacity-0 translate-y-8 hero-anim-item">
                <div class="relative inline-flex items-center justify-center p-3 rounded-full border border-luxuryRed/40 bg-luxuryDark-card/50 glow-border-red">
                    <svg class="w-8 h-8 text-luxuryRed-light animate-spin" style="animation-duration: 8s;" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <circle cx="12" cy="12" r="10" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
                        <path d="M12 2v20M2 12h20" stroke="currentColor" stroke-width="0.5"/>
                    </svg>
                    <i class="fa-solid fa-atom absolute text-sm text-luxuryRed-light"></i>
                </div>
            </div>

            <!-- Pre-title -->
            <span class="text-xs md:text-sm font-semibold uppercase tracking-[0.4em] text-luxuryRed-light mb-4 block opacity-0 translate-y-8 hero-anim-item">
                MÓN QUÀ TRI ÂN THÁNG SÁU
            </span>

            <!-- Main Title -->
            <h1 class="font-serif text-4xl sm:text-6xl md:text-8xl font-bold tracking-tight text-white mb-6 leading-tight opacity-0 translate-y-8 hero-anim-item">
                Tri Ân Người Thầy <br>
                <span class="italic font-normal text-transparent bg-clip-text bg-gradient-to-r from-white via-red-200 to-luxuryRed-light glow-text-red">Đặc Biệt</span>
            </h1>

            <!-- Subtitle -->
            <p class="text-base sm:text-lg md:text-xl text-neutral-300 max-w-3xl leading-relaxed mb-4 font-light opacity-0 translate-y-8 hero-anim-item">
                Gửi đến <strong class="text-white font-semibold glow-text-red">Thầy Vũ Tá Quyền</strong> — người thầy vĩ đại đã thắp sáng ngọn lửa đam mê Vật Lý và đồng hành cùng em trong suốt hành trình 3 năm thanh xuân cấp ba đầy hoài bão.
            </p>

            <!-- From line -->
            <p class="text-sm italic text-neutral-400 mb-10 opacity-0 translate-y-8 hero-anim-item">
                Bày tỏ sâu sắc bởi học trò: <span class="text-luxuryRed-light font-semibold not-italic">Phan Hòa Phát</span>
            </p>

            <!-- Buttons -->
            <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-6 opacity-0 translate-y-8 hero-anim-item">
                <a href="#intro" class="bg-gradient-to-r from-luxuryRed to-luxuryRed-light text-white font-bold px-8 py-4 rounded-full shadow-[0_0_20px_rgba(255,45,85,0.4)] hover:shadow-[0_0_35px_rgba(255,45,85,0.8)] transition-all duration-300 transform hover:-translate-y-1 text-center min-w-[200px] border border-white/10">
                    Bắt đầu hành trình <i class="fa-solid fa-arrow-right ml-2 text-sm"></i>
                </a>
                <a href="#wishes" class="bg-luxuryDark-card border border-luxuryRed/40 text-neutral-200 font-semibold px-8 py-4 rounded-full hover:bg-luxuryRed/10 hover:text-white hover:border-luxuryRed-light transition-all duration-300 text-center min-w-[200px]">
                    Những Điều Muốn Gửi
                </a>
            </div>
        </div>

        <!-- Scroll Indicator -->
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex flex-col items-center pointer-events-none opacity-0" id="scroll-indicator">
            <span class="text-[10px] tracking-[0.3em] uppercase text-neutral-400 mb-2">Cuộn để xem</span>
            <div class="w-[1.5px] h-12 bg-neutral-800 relative overflow-hidden rounded">
                <div class="absolute top-0 left-0 w-full h-1/2 bg-luxuryRed-light rounded" id="scroll-wheel"></div>
            </div>
        </div>
    </section>

    <!-- -->
    <!-- 2. SECTION GIỚI THIỆU THẦY (PHYSICS ENERGY) -->
    <section id="intro" class="py-24 relative z-20 px-4 md:px-8">
        <div class="max-w-6xl mx-auto">
            <!-- Section Header -->
            <div class="text-center mb-16 scroll-anim-header">
                <span class="text-xs uppercase tracking-[0.3em] text-luxuryRed-light font-semibold">The Light of Knowledge</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold mt-2 text-white">Chân Dung Người Thầy Vật Lý</h2>
                <div class="w-16 h-1 bg-luxuryRed mx-auto mt-4 rounded-full shadow-[0_0_8px_#ff2d55]"></div>
            </div>

            <!-- Content Grid with Luxury Card -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Left Side: Interactive Physics Visualization -->
                <div class="lg:col-span-5 flex justify-center relative scroll-anim-left">
                    <div class="absolute w-72 h-72 bg-luxuryRed/10 rounded-full blur-3xl"></div>
                    <!-- Outer Orbit Box -->
                    <div class="relative w-80 h-80 rounded-full border border-luxuryRed/30 flex items-center justify-center p-8 glow-border-red physics-float">
                        <!-- Orbit Ring 1 -->
                        <div class="absolute w-full h-full rounded-full border border-dashed border-luxuryRed-light/25 animate-spin" style="animation-duration: 18s;"></div>
                        <!-- Orbit Ring 2 -->
                        <div class="absolute w-[80%] h-[80%] rounded-full border border-double border-luxuryRed/40 animate-spin" style="animation-duration: 10s; animation-direction: reverse;"></div>
                        
                        <!-- Center Core -->
                        <div class="w-48 h-48 rounded-full bg-gradient-to-br from-luxuryDark-card to-luxuryRed/25 flex flex-col items-center justify-center text-center p-4 border border-luxuryRed-light/30 shadow-2xl relative z-10">
                            <!-- Atom SVGs orbiting -->
                            <i class="fa-solid fa-atom text-4xl text-luxuryRed-light mb-3 animate-pulse"></i>
                            <span class="text-lg font-serif font-semibold tracking-wider text-white">Vật Lý Vũ Trụ</span>
                            <span class="text-[10px] text-neutral-400 mt-1 uppercase tracking-widest">Lực hấp dẫn trí tuệ</span>
                        </div>

                        <!-- Mini Particle Nodes floating around -->
                        <div class="absolute top-[10%] left-[20%] w-3 h-3 bg-luxuryRed-light rounded-full animate-bounce"></div>
                        <div class="absolute bottom-[15%] right-[10%] w-4 h-4 bg-red-400 rounded-full animate-pulse"></div>
                        <div class="absolute top-[75%] left-[10%] w-2 h-2 bg-white rounded-full"></div>
                    </div>
                </div>

                <!-- Right Side: Luxury Introduction Card -->
                <div class="lg:col-span-7 scroll-anim-right">
                    <div class="luxury-glass p-8 md:p-12 rounded-3xl relative overflow-hidden group">
                        <!-- Subtle corner light sweep -->
                        <div class="absolute top-0 left-0 w-32 h-32 bg-gradient-to-br from-luxuryRed-light/20 to-transparent blur-xl pointer-events-none"></div>
                        
                        <div class="flex items-center space-x-4 mb-6">
                            <span class="bg-luxuryRed/30 text-luxuryRed-light font-bold px-4 py-1.5 rounded-full text-xs uppercase tracking-wider border border-luxuryRed-light/30">
                                Người Thầy Truyền Cảm Hứng
                            </span>
                        </div>

                        <h3 class="font-serif text-3xl md:text-4xl font-bold text-white mb-2 tracking-wide group-hover:text-luxuryRed-light transition-colors duration-300">
                            Thầy Vũ Tá Quyền
                        </h3>
                        <p class="text-luxuryRed-light text-sm font-semibold uppercase tracking-widest mb-6">
                            Giáo viên Vật Lý bậc THPT
                        </p>

                        <div class="space-y-6 text-neutral-300 leading-relaxed font-light text-base md:text-lg">
                            <p>
                                Một người thầy năng động, đầy nhiệt huyết, sáng tạo và luôn mang đến nguồn năng lượng tích cực bùng nổ trong từng tiết học. Đối với tụi em, những bài học cơ học, điện trường, hay quang học không còn là những công thức khô khan của những con số vô hồn.
                            </p>
                            <p class="border-l-2 border-luxuryRed-light pl-4 italic text-neutral-200 bg-luxuryRed/5 py-2 pr-2 rounded-r-lg">
                                "Thầy biến những định luật Newton hay thuyết tương đối phức tạp thành những bài ca, những câu chuyện thực tiễn đầy lôi cuốn."
                            </p>
                            <p>
                                Không chỉ dừng lại ở việc giúp học sinh thấu hiểu sâu sắc kiến thức, thầy Vũ Tá Quyền còn là người thắp lửa, truyền động lực vượt trội, dạy tụi em sự tự tin và khơi dậy niềm đam mê mãnh liệt đối với môn học mang tính vũ trụ này.
                            </p>
                        </div>

                        <!-- Small Physics Metric Stats -->
                        <div class="grid grid-cols-3 gap-4 mt-8 pt-8 border-t border-luxuryRed/20">
                            <div class="text-center">
                                <div class="font-serif text-2xl md:text-3xl font-bold text-white glow-text-red">3</div>
                                <div class="text-[10px] uppercase text-neutral-400 tracking-wider mt-1">Năm Đồng Hành</div>
                            </div>
                            <div class="text-center">
                                <div class="font-serif text-2xl md:text-3xl font-bold text-white glow-text-red">1000+</div>
                                <div class="text-[10px] uppercase text-neutral-400 tracking-wider mt-1">Bài Giảng Hay</div>
                            </div>
                            <div class="text-center">
                                <div class="font-serif text-2xl md:text-3xl font-bold text-white glow-text-red">∞</div>
                                <div class="text-[10px] uppercase text-neutral-400 tracking-wider mt-1">Ngọn Lửa Đam Mê</div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- -->
    <!-- 3. SECTION LỜI CẢM ƠN (QUOTE CARDS) -->
    <section id="gratitude" class="py-24 relative z-20 px-4 md:px-8 bg-gradient-to-b from-transparent via-luxuryDark-card/40 to-transparent">
        <div class="max-w-6xl mx-auto">
            <!-- Header -->
            <div class="text-center mb-16 scroll-anim-header">
                <span class="text-xs uppercase tracking-[0.3em] text-luxuryRed-light font-semibold">Our Heartfelt Thank You</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold mt-2 text-white">Những Lời Cảm Ơn Sâu Sắc nhất</h2>
                <div class="w-16 h-1 bg-luxuryRed mx-auto mt-4 rounded-full shadow-[0_0_8px_#ff2d55]"></div>
            </div>

            <!-- Quotes Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Quote 1 -->
                <div class="luxury-glass p-8 md:p-10 rounded-2xl relative overflow-hidden group scroll-anim-up">
                    <div class="absolute -right-4 -top-4 opacity-5 group-hover:opacity-10 transition-opacity duration-300">
                        <i class="fa-solid fa-quote-right text-9xl text-luxuryRed-light"></i>
                    </div>
                    <div class="flex items-start space-x-4">
                        <span class="text-luxuryRed-light text-2xl mt-1"><i class="fa-solid fa-circle-check"></i></span>
                        <div>
                            <h4 class="font-serif text-xl font-bold text-white mb-3">Cảm ơn vì 3 năm đồng hành vàng ngọc</h4>
                            <p class="text-neutral-300 font-light leading-relaxed">
                                Cảm ơn thầy vì đã luôn kiên nhẫn, bền bỉ sát cánh cùng em qua mọi kì kiểm tra, mọi tiết học căng thẳng của 3 năm trung học phổ thông. Sự nâng đỡ của thầy là bệ phóng lớn cho em tiến bước tương lai.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Quote 2 -->
                <div class="luxury-glass p-8 md:p-10 rounded-2xl relative overflow-hidden group scroll-anim-up" style="transition-delay: 150ms;">
                    <div class="absolute -right-4 -top-4 opacity-5 group-hover:opacity-10 transition-opacity duration-300">
                        <i class="fa-solid fa-quote-right text-9xl text-luxuryRed-light"></i>
                    </div>
                    <div class="flex items-start space-x-4">
                        <span class="text-luxuryRed-light text-2xl mt-1"><i class="fa-solid fa-fire-flame-curved"></i></span>
                        <div>
                            <h4 class="font-serif text-xl font-bold text-white mb-3">Nhiệt huyết cháy bỏng trong từng lời giảng</h4>
                            <p class="text-neutral-300 font-light leading-relaxed">
                                Cảm ơn thầy vì những bài giảng Vật Lý đầy bùng nổ, luôn ngập tràn nhiệt huyết và sự sáng tạo. Thầy đã chứng minh cho em thấy khoa học không chỉ là lý thuyết, đó là sự kỳ diệu của thực tại.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Quote 3 -->
                <div class="luxury-glass p-8 md:p-10 rounded-2xl relative overflow-hidden group scroll-anim-up" style="transition-delay: 300ms;">
                    <div class="absolute -right-4 -top-4 opacity-5 group-hover:opacity-10 transition-opacity duration-300">
                        <i class="fa-solid fa-quote-right text-9xl text-luxuryRed-light"></i>
                    </div>
                    <div class="flex items-start space-x-4">
                        <span class="text-luxuryRed-light text-2xl mt-1"><i class="fa-solid fa-face-smile-beam"></i></span>
                        <div>
                            <h4 class="font-serif text-xl font-bold text-white mb-3">Những nụ cười giải tỏa áp lực học đường</h4>
                            <p class="text-neutral-300 font-light leading-relaxed">
                                Cảm ơn thầy vì tính cách vô cùng gần gũi, dễ thương và luôn biết cách mang lại những tràng cười sảng khoái cho chúng em. Những trò đùa thông thái của thầy là "chất xúc tác" tuyệt vời nhất.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Quote 4 -->
                <div class="luxury-glass p-8 md:p-10 rounded-2xl relative overflow-hidden group scroll-anim-up" style="transition-delay: 450ms;">
                    <div class="absolute -right-4 -top-4 opacity-5 group-hover:opacity-10 transition-opacity duration-300">
                        <i class="fa-solid fa-quote-right text-9xl text-luxuryRed-light"></i>
                    </div>
                    <div class="flex items-start space-x-4">
                        <span class="text-luxuryRed-light text-2xl mt-1"><i class="fa-solid fa-seedling"></i></span>
                        <div>
                            <h4 class="font-serif text-xl font-bold text-white mb-3">Vật Lý - Một phần thanh xuân đáng nhớ</h4>
                            <p class="text-neutral-300 font-light leading-relaxed">
                                Những tiết học Vật Lý của thầy Vũ Tá Quyền đã vượt xa ranh giới của một môn học đơn thuần. Đó đã trở thành một phần ký ức thanh xuân rực rỡ nhất mà em luôn mang theo trong suốt cuộc đời.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- -->
    <!-- 4. SECTION KỶ NIỆM THANH XUÂN (TIMELINE) -->
    <section id="timeline" class="py-24 relative z-20 px-4 md:px-8">
        <div class="max-w-4xl mx-auto">
            <!-- Header -->
            <div class="text-center mb-20 scroll-anim-header">
                <span class="text-xs uppercase tracking-[0.3em] text-luxuryRed-light font-semibold">Memories Through Time</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold mt-2 text-white">Hành Trình Kỷ Niệm 3 Năm</h2>
                <div class="w-16 h-1 bg-luxuryRed mx-auto mt-4 rounded-full shadow-[0_0_8px_#ff2d55]"></div>
            </div>

            <!-- Cinematic Vertical Timeline -->
            <div class="relative border-l border-luxuryRed/30 ml-4 md:ml-32 py-4">
                
                <!-- Timeline Element 1 -->
                <div class="mb-16 relative pl-8 md:pl-12 scroll-anim-up">
                    <!-- Timeline Dot with Glow -->
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-luxuryRed border border-luxuryRed-light glow-border-red flex items-center justify-center">
                        <div class="w-2 h-2 rounded-full bg-white"></div>
                    </div>
                    <!-- Year Badge (Absolute Left on Desktop) -->
                    <div class="hidden md:block absolute right-full mr-12 top-0 text-right">
                        <span class="font-serif text-2xl font-bold text-white tracking-widest glow-text-red">NĂM LỚP 10</span>
                        <p class="text-[10px] tracking-widest text-neutral-400 uppercase mt-1">Bắt đầu chặng đường</p>
                    </div>
                    <!-- Card content -->
                    <div class="luxury-glass p-6 md:p-8 rounded-2xl group transition-all duration-300 hover:translate-x-2">
                        <span class="md:hidden text-xs font-bold text-luxuryRed-light uppercase block mb-2">Năm Lớp 10 • Những ngày đầu tiên</span>
                        <h3 class="font-serif text-xl font-bold text-white mb-3">Cuộc Gặp Gỡ Định Mệnh & Làm Quen Vật Lý</h3>
                        <p class="text-neutral-300 font-light leading-relaxed">
                            Những ngày đầu bước chân vào trường THPT còn nhiều bỡ ngỡ, những tiết học Vật Lý đầy ắp sự lôi cuốn của thầy đã gạt bỏ nỗi sợ hãi. Sự dí dỏm cùng nguồn năng lượng mạnh mẽ phát ra từ thầy thu hút em ngay lập tức.
                        </p>
                    </div>
                </div>

                <!-- Timeline Element 2 -->
                <div class="mb-16 relative pl-8 md:pl-12 scroll-anim-up" style="transition-delay: 100ms;">
                    <!-- Timeline Dot -->
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-luxuryRed border border-luxuryRed-light glow-border-red flex items-center justify-center">
                        <div class="w-2 h-2 rounded-full bg-white"></div>
                    </div>
                    <!-- Year Badge -->
                    <div class="hidden md:block absolute right-full mr-12 top-0 text-right">
                        <span class="font-serif text-2xl font-bold text-white tracking-widest glow-text-red">NĂM LỚP 11</span>
                        <p class="text-[10px] tracking-widest text-neutral-400 uppercase mt-1">Gắn kết & Vượt bão</p>
                    </div>
                    <!-- Card content -->
                    <div class="luxury-glass p-6 md:p-8 rounded-2xl group transition-all duration-300 hover:translate-x-2">
                        <span class="md:hidden text-xs font-bold text-luxuryRed-light uppercase block mb-2">Năm Lớp 11 • Gắn kết say mê</span>
                        <h3 class="font-serif text-xl font-bold text-white mb-3">Bùng Nổ Tri Thức & Say Mê Sáng Tạo</h3>
                        <p class="text-neutral-300 font-light leading-relaxed">
                            Năm học tăng tốc với nhiều bài học khó hơn. Nhưng bằng khả năng giảng dạy biến chuyển thần sầu, thầy đã đưa lớp chúng em chinh phục các chuyên đề hóc búa nhất. Tiếng cười trong lớp dường như chưa bao giờ dứt.
                        </p>
                    </div>
                </div>

                <!-- Timeline Element 3 -->
                <div class="mb-16 relative pl-8 md:pl-12 scroll-anim-up" style="transition-delay: 200ms;">
                    <!-- Timeline Dot -->
                    <div class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-luxuryRed border border-luxuryRed-light glow-border-red flex items-center justify-center">
                        <div class="w-2 h-2 rounded-full bg-white"></div>
                    </div>
                    <!-- Year Badge -->
                    <div class="hidden md:block absolute right-full mr-12 top-0 text-right">
                        <span class="font-serif text-2xl font-bold text-white tracking-widest glow-text-red">NĂM LỚP 12</span>
                        <p class="text-[10px] tracking-widest text-neutral-400 uppercase mt-1">Thanh xuân cuối cấp</p>
                    </div>
                    <!-- Card content -->
                    <div class="luxury-glass p-6 md:p-8 rounded-2xl group transition-all duration-300 hover:translate-x-2">
                        <span class="md:hidden text-xs font-bold text-luxuryRed-light uppercase block mb-2">Năm Lớp 12 • Chặng đường cuối</span>
                        <h3 class="font-serif text-xl font-bold text-white mb-3">Tăng Tốc Vượt Vũ Môn & Trưởng Thành</h3>
                        <p class="text-neutral-300 font-light leading-relaxed">
                            Năm học bận rộn nhất với những kỳ thi cam go và áp lực lớn. Lớp học của thầy Vũ Tá Quyền chính là nơi tiếp thêm nguồn dưỡng chất tinh thần vô giá để tụi em trút bỏ áp lực, sẵn sàng sải cánh bay vào những khoảng trời xa xôi.
                        </p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- -->
    <!-- 5. SECTION LỜI CHÚC ĐẾN THẦY + 6. HIỆU ỨNG TRÁI TIM TƯƠNG TÁC -->
    <section id="wishes" class="py-24 relative z-20 px-4 md:px-8 bg-gradient-to-t from-black via-luxuryDark-card to-transparent">
        <div class="max-w-4xl mx-auto text-center relative">
            
            <!-- Section Header -->
            <div class="mb-12 scroll-anim-header">
                <span class="text-xs uppercase tracking-[0.3em] text-luxuryRed-light font-semibold">A Student's Ultimate Wish</span>
                <h2 class="font-serif text-3xl md:text-5xl font-bold mt-2 text-white">Lời Chúc Chân Thành Gửi Thầy</h2>
                <div class="w-16 h-1 bg-luxuryRed mx-auto mt-4 rounded-full shadow-[0_0_8px_#ff2d55]"></div>
            </div>

            <!-- Big Emotional Card with Light sweep effect -->
            <div class="luxury-glass p-8 md:p-14 rounded-3xl relative overflow-hidden shadow-2xl border border-luxuryRed/30 scroll-anim-up">
                
                <!-- Light Sweep Overlay -->
                <div class="absolute inset-0 bg-gradient-to-r from-transparent via-white/5 to-transparent -translate-x-full transition-transform duration-1000 ease-in-out pointer-events-none" id="light-sweep"></div>
                
                <!-- Quote mark watermark -->
                <span class="absolute top-6 left-6 text-neutral-800/60 text-7xl font-serif pointer-events-none">“</span>

                <div class="relative z-10">
                    <!-- Wish Text -->
                    <p class="font-serif text-xl md:text-3xl font-light italic text-neutral-100 leading-relaxed mb-10 text-center">
                        "Em xin kính chúc <span class="text-white font-bold not-italic glow-text-red">Thầy Vũ Tá Quyền</span> luôn ngập tràn sức khỏe, ngập tràn hạnh phúc và mãi mãi giữ vững ngọn lửa nhiệt huyết rực cháy với nghề giáo cao quý. Mong rằng thầy sẽ gặt hái thật nhiều thành công rực rỡ và tiếp tục truyền cảm hứng tươi đẹp cho hàng nghìn thế hệ học sinh mai sau."
                    </p>

                    <!-- Student Signature -->
                    <div class="flex flex-col items-center justify-center mt-6">
                        <div class="w-12 h-[1px] bg-luxuryRed mb-3"></div>
                        <span class="text-xs text-neutral-400 uppercase tracking-[0.3em] mb-1">Học trò luôn biết ơn và kính trọng thầy</span>
                        <span class="font-serif text-2xl font-bold text-white tracking-widest glow-text-red italic">Phan Hòa Phát</span>
                    </div>

                    <!-- Heart Interactive Area -->
                    <div class="mt-12 flex flex-col items-center justify-center">
                        <p class="text-xs text-neutral-400 uppercase tracking-widest mb-4">Nhấp vào trái tim để gửi ngàn tia tri ân</p>
                        
                        <!-- The Special Interactive Heart Container -->
                        <div class="relative flex items-center justify-center w-40 h-40" id="heart-container">
                            <!-- Burst Canvas specifically for this button (centered with translate) -->
                            <canvas id="heart-burst-canvas" class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[300px] h-[300px] pointer-events-none z-10"></canvas>
                            
                            <!-- Heart button -->
                            <button id="heart-btn" class="w-20 h-20 bg-gradient-to-br from-luxuryRed to-luxuryRed-light rounded-full flex items-center justify-center shadow-[0_0_20px_rgba(255,45,85,0.6)] hover:shadow-[0_0_40px_rgba(255,45,85,1)] hover:scale-110 active:scale-95 transition-all duration-300 z-20 cursor-pointer pulse-active">
                                <i class="fa-solid fa-heart text-white text-3xl"></i>
                            </button>
                        </div>
                        
                        <p class="text-xs text-luxuryRed-light font-semibold tracking-wider mt-4 opacity-0 transition-opacity duration-500" id="tap-message">
                            Nhịp tim biết ơn đã lan tỏa vào vũ trụ! ❤️
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="py-12 border-t border-luxuryRed/10 relative z-20 bg-black text-center">
        <div class="max-w-6xl mx-auto px-4 flex flex-col items-center">
            <!-- Icon -->
            <div class="text-luxuryRed-light text-2xl mb-4">
                <i class="fa-solid fa-heart"></i>
            </div>
            <!-- Credits -->
            <p class="font-serif text-lg text-white tracking-widest mb-2">
                FROM PHAN HÒA PHÁT
            </p>
            <p class="text-xs text-neutral-500 uppercase tracking-widest mb-6">
                With Deepest Respect & Gratitude to Thầy Vũ Tá Quyền
            </p>
            <!-- Copy -->
            <p class="text-[10px] text-neutral-600">
                &copy; 2026. Made with love and physics logic by Phan Hòa Phát.
            </p>
        </div>
    </footer>

    <!-- -->
    <!-- INTERACTION LOGIC & EFFECTS -->
    <script>
        
        // --- GLOBAL BACKGROUND PARTICLES CANVAS ---
        const canvas = document.getElementById('particles-canvas');
        const ctx = canvas.getContext('2d');

        let particlesArray = [];
        const numberOfParticles = 75;

        // Resize Canvas to fill screen properly with High-DPI support
        function resizeCanvas() {
            const dpr = window.devicePixelRatio || 1;
            canvas.width = window.innerWidth * dpr;
            canvas.height = window.innerHeight * dpr;
            canvas.style.width = `${window.innerWidth}px`;
            canvas.style.height = `${window.innerHeight}px`;
            ctx.scale(dpr, dpr);
            
            initParticles();
        }

        class Particle {
            constructor() {
                this.x = Math.random() * window.innerWidth;
                this.y = Math.random() * window.innerHeight;
                this.size = Math.random() * 2 + 0.5;
                this.speedX = (Math.random() - 0.5) * 0.35;
                this.speedY = (Math.random() - 0.5) * 0.35 - 0.15; // Soft upward vector
                this.alpha = Math.random() * 0.6 + 0.2;
                this.color = `rgba(255, ${Math.floor(Math.random() * 50 + 10)}, ${Math.floor(Math.random() * 60 + 10)}, `;
            }

            update() {
                this.x += this.speedX;
                this.y += this.speedY;

                // Wrap around logic
                if (this.y < 0) {
                    this.y = window.innerHeight;
                    this.x = Math.random() * window.innerWidth;
                }
                if (this.x < 0) this.x = window.innerWidth;
                if (this.x > window.innerWidth) this.x = 0;
            }

            draw() {
                ctx.save();
                ctx.globalAlpha = this.alpha;
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                ctx.fillStyle = this.color + '1)';
                ctx.shadowBlur = 6;
                ctx.shadowColor = '#ff2d55';
                ctx.fill();
                ctx.restore();
            }
        }

        function initParticles() {
            particlesArray = [];
            for (let i = 0; i < numberOfParticles; i++) {
                particlesArray.push(new Particle());
            }
        }

        function animateParticles() {
            ctx.clearRect(0, 0, window.innerWidth, window.innerHeight);
            for (let i = 0; i < particlesArray.length; i++) {
                particlesArray[i].update();
                particlesArray[i].draw();
            }
            requestAnimationFrame(animateParticles);
        }

        window.addEventListener('resize', resizeCanvas);
        resizeCanvas();
        animateParticles();


        //        // --- CUSTOM CURSOR LOGIC WITH ENHANCED SENSITIVITY ---
        const cursorDot = document.getElementById('cursor-dot');
        const cursorOutline = document.getElementById('cursor-outline');
        let cursorInitialized = false;

        window.addEventListener('mousemove', (e) => {
            const posX = e.clientX;
            const posY = e.clientY;

            // Make cursor visible on first movement inside the window
            if (!cursorInitialized) {
                cursorDot.style.opacity = '1';
                cursorOutline.style.opacity = '1';
                cursorInitialized = true;
            }

            cursorDot.style.left = `${posX}px`;
            cursorDot.style.top = `${posY}px`;

            gsap.to(cursorOutline, {
                duration: 0.15,
                left: posX,
                top: posY,
                ease: 'power2.out'
            });
        });

        // Hide when mouse exits viewport
        document.addEventListener('mouseleave', () => {
            cursorDot.style.opacity = '0';
            cursorOutline.style.opacity = '0';
            cursorInitialized = false;
        });

        document.addEventListener('mouseenter', () => {
            cursorDot.style.opacity = '1';
            cursorOutline.style.opacity = '1';
            cursorInitialized = true;
        });

        // Hover expansions for premium links/elements
        const hoverables = document.querySelectorAll('a, button, .luxury-glass, #heart-btn');
        hoverables.forEach(item => {
            item.addEventListener('mouseenter', () => {
                cursorDot.style.width = '14px';
                cursorDot.style.height = '14px';
                cursorOutline.style.transform = 'translate(-50%, -50%) scale(1.5)';
                cursorOutline.style.borderColor = '#ff2d55';
                cursorOutline.style.backgroundColor = 'rgba(255, 45, 85, 0.08)';
            });
            item.addEventListener('mouseleave', () => {
                cursorDot.style.width = '8px';
                cursorDot.style.height = '8px';
                cursorOutline.style.transform = 'translate(-50%, -50%) scale(1)';
                cursorOutline.style.borderColor = 'rgba(255, 45, 85, 0.5)';
                cursorOutline.style.backgroundColor = 'transparent';
            });
        });


        //        // --- HEART EXPLOSION CANVAS EFFECT (SEC 6) ---
        const heartCanvas = document.getElementById('heart-burst-canvas');
        const hctx = heartCanvas.getContext('2d');
        let heartParticles = [];

        // Set High-DPI Resolution for the Canvas
        function resizeHeartCanvas() {
            const dpr = window.devicePixelRatio || 1;
            heartCanvas.width = 300 * dpr;
            heartCanvas.height = 300 * dpr;
            heartCanvas.style.width = '300px';
            heartCanvas.style.height = '300px';
            hctx.scale(dpr, dpr);
        }
        resizeHeartCanvas();

        class HeartParticle {
            constructor(x, y) {
                this.x = x;
                this.y = y;
                this.size = Math.random() * 3.5 + 1.5;
                // Perfect physics vector dispersal
                const angle = Math.random() * Math.PI * 2;
                const speed = Math.random() * 3.5 + 1.5;
                this.speedX = Math.cos(angle) * speed;
                this.speedY = Math.sin(angle) * speed - 0.5; // Slight upward velocity gravity compensation
                this.gravity = 0.04;
                this.color = `hsl(${Math.random() * 25 + 340}, 100%, ${Math.random() * 20 + 50}%)`; 
                this.alpha = 1;
                this.decay = Math.random() * 0.015 + 0.01;
            }

            update() {
                this.x += this.speedX;
                this.y += this.speedY;
                this.speedY += this.gravity;
                this.alpha -= this.decay;
            }

            draw() {
                hctx.save();
                hctx.globalAlpha = this.alpha;
                hctx.beginPath();
                hctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                hctx.fillStyle = this.color;
                hctx.shadowBlur = 8;
                hctx.shadowColor = '#ff1a1a';
                hctx.fill();
                hctx.restore();
            }
        }

        function createBurst() {
            const centerX = 150; // Coordinates are half of 300 in non-dpr scale
            const centerY = 150;
            for (let i = 0; i < 45; i++) {
                heartParticles.push(new HeartParticle(centerX, centerY));
            }
        }

        function animateHeartParticles() {
            hctx.clearRect(0, 0, 300, 300);
            for (let i = 0; i < heartParticles.length; i++) {
                heartParticles[i].update();
                heartParticles[i].draw();
                
                if (heartParticles[i].alpha <= 0) {
                    heartParticles.splice(i, 1);
                    i--;
                }
            }
            requestAnimationFrame(animateHeartParticles);
        }
        animateHeartParticles();


        // Interactive triggers
        const heartBtn = document.getElementById('heart-btn');
        const heartContainer = document.getElementById('heart-container');
        const tapMessage = document.getElementById('tap-message');
        const lightSweep = document.getElementById('light-sweep');

        // Physics Formulas & Emojis list to spawn on click
        const floaters = ['❤️', '✨', 'V.T.Q', 'F=ma', 'E=mc²', '⚛️'];

        heartBtn.addEventListener('click', () => {
            // Burst Canvas Particles
            createBurst();
            
            // Spawn floaters dynamically
            for (let i = 0; i < 3; i++) {
                const floater = document.createElement('div');
                floater.classList.add('floating-heart-emoji');
                floater.innerText = floaters[Math.floor(Math.random() * floaters.length)];
                floater.style.setProperty('--random-x', `${(Math.random() - 0.5) * 80}px`);
                floater.style.setProperty('--random-rotate', `${(Math.random() - 0.5) * 40}deg`);
                
                // Position randomly around button center
                floater.style.left = `calc(50% + ${(Math.random() - 0.5) * 40}px - 12px)`;
                floater.style.top = `calc(50% - 12px)`;
                
                heartContainer.appendChild(floater);
                
                // Cleanup floaters after animation ends
                setTimeout(() => {
                    floater.remove();
                }, 1200);
            }

            // Message trigger
            tapMessage.classList.remove('opacity-0');
            tapMessage.classList.add('opacity-100');

            // Ambient card illumination swipe
            lightSweep.style.transform = 'translateX(100%)';
            setTimeout(() => {
                lightSweep.style.transform = 'translateX(-100%)';
            }, 1000);

            // Pop scale logic using GSAP
            gsap.fromTo(heartBtn, 
                { scale: 0.8 }, 
                { scale: 1.1, duration: 0.45, ease: 'elastic.out(1.2, 0.4)' }
            );
        });


        //        // --- GSAP SCROLL TRIGGER ANIMATIONS & NAVIGATION ---
        gsap.registerPlugin(ScrollTrigger);

        window.addEventListener('DOMContentLoaded', () => {
            // Smoothly reveal Hero content
            gsap.to('.hero-anim-item', {
                opacity: 1,
                y: 0,
                duration: 1.4,
                stagger: 0.12,
                ease: 'power4.out',
                delay: 0.2
            });

            gsap.to('#scroll-indicator', {
                opacity: 1,
                duration: 1,
                delay: 1.8
            });

            gsap.to('#scroll-wheel', {
                y: 20,
                repeat: -1,
                duration: 1.4,
                ease: 'power2.inOut',
                yoyo: true
            });
        });

        // Synchronize scroll-progress indicator
        window.addEventListener('scroll', () => {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            const scrolled = (winScroll / height) * 100;
            document.getElementById('scroll-progress').style.width = scrolled + '%';

            // Shrink navbar & raise contrast on scroll
            const header = document.querySelector('header');
            if (window.scrollY > 40) {
                header.classList.add('py-2');
                header.querySelector('nav').style.backgroundColor = 'rgba(10, 3, 3, 0.9)';
            } else {
                header.classList.remove('py-2');
                header.querySelector('nav').style.backgroundColor = 'rgba(22, 10, 10, 0.45)';
            }
        });

        // Cinematic scrolling headers animation
        const headers = document.querySelectorAll('.scroll-anim-header');
        headers.forEach(header => {
            gsap.from(header, {
                scrollTrigger: {
                    trigger: header,
                    start: 'top 85%',
                    toggleActions: 'play none none none'
                },
                opacity: 0,
                y: 40,
                duration: 1.1,
                ease: 'power3.out'
            });
        });

        // Entrance animation: Intro physics
        gsap.from('.scroll-anim-left', {
            scrollTrigger: {
                trigger: '.scroll-anim-left',
                start: 'top 80%'
            },
            opacity: 0,
            x: -50,
            duration: 1.2,
            ease: 'power3.out'
        });

        gsap.from('.scroll-anim-right', {
            scrollTrigger: {
                trigger: '.scroll-anim-right',
                start: 'top 80%'
            },
            opacity: 0,
            x: 50,
            duration: 1.2,
            ease: 'power3.out'
        });

        // Entrance animation: Generic reveal
        const upReveals = document.querySelectorAll('.scroll-anim-up');
        upReveals.forEach(el => {
            gsap.from(el, {
                scrollTrigger: {
                    trigger: el,
                    start: 'top 85%'
                },
                opacity: 0,
                y: 50,
                duration: 1.1,
                ease: 'power3.out'
            });
        });

    </script>
</body>
</html>
