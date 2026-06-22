<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>DevPulse | Vibrant Developer Profile</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
            display: inline-block;
            vertical-align: middle;
        }
        .vibrant-gradient {
            background: linear-gradient(135deg, #4648d4 0%, #6063ee 50%, #006c49 100%);
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "tertiary": "#825100",
                        "on-secondary": "#ffffff",
                        "outline": "#767586",
                        "surface-container-lowest": "#ffffff",
                        "on-tertiary-fixed": "#2a1700",
                        "on-primary-fixed-variant": "#2f2ebe",
                        "on-error": "#ffffff",
                        "primary": "#4648d4",
                        "secondary": "#006c49",
                        "on-tertiary": "#ffffff",
                        "on-error-container": "#93000a",
                        "primary-fixed-dim": "#c0c1ff",
                        "error": "#ba1a1a",
                        "on-background": "#0b1c30",
                        "inverse-primary": "#c0c1ff",
                        "on-primary-fixed": "#07006c",
                        "error-container": "#ffdad6",
                        "secondary-container": "#6cf8bb",
                        "on-secondary-container": "#00714d",
                        "tertiary-fixed-dim": "#ffb95f",
                        "surface-bright": "#f8f9ff",
                        "on-primary-container": "#fffbff",
                        "surface": "#f8f9ff",
                        "surface-container-highest": "#d3e4fe",
                        "surface-container-low": "#eff4ff",
                        "on-tertiary-container": "#fffbff",
                        "on-secondary-fixed": "#002113",
                        "surface-dim": "#cbdbf5",
                        "primary-fixed": "#e1e0ff",
                        "on-secondary-fixed-variant": "#005236",
                        "outline-variant": "#c7c4d7",
                        "surface-container": "#e5eeff",
                        "inverse-on-surface": "#eaf1ff",
                        "primary-container": "#6063ee",
                        "on-tertiary-fixed-variant": "#653e00",
                        "on-surface-variant": "#464554",
                        "surface-tint": "#494bd6",
                        "inverse-surface": "#213145",
                        "tertiary-container": "#a36700",
                        "secondary-fixed-dim": "#4edea3",
                        "on-surface": "#0b1c30",
                        "background": "#f8f9ff",
                        "surface-variant": "#d3e4fe",
                        "secondary-fixed": "#6ffbbe",
                        "surface-container-high": "#dce9ff",
                        "on-primary": "#ffffff",
                        "tertiary-fixed": "#ffddb8"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "spacing": {
                        "sm": "8px",
                        "container-max": "1280px",
                        "gutter": "24px",
                        "lg": "24px",
                        "base": "4px",
                        "xl": "40px",
                        "xs": "4px",
                        "md": "16px"
                    },
                    "fontFamily": {
                        "body-sm": ["Inter"],
                        "headline-xl": ["Inter"],
                        "label-sm": ["Inter"],
                        "label-md": ["Inter"],
                        "body-md": ["Inter"],
                        "headline-lg": ["Inter"],
                        "headline-md": ["Inter"],
                        "body-lg": ["Inter"]
                    },
                    "fontSize": {
                        "body-sm": ["14px", {"lineHeight": "20px", "fontWeight": "400"}],
                        "headline-xl": ["36px", {"lineHeight": "44px", "letterSpacing": "-0.02em", "fontWeight": "700"}],
                        "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.02em", "fontWeight": "500"}],
                        "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "600"}],
                        "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                        "headline-md": ["20px", {"lineHeight": "28px", "fontWeight": "600"}],
                        "headline-lg": ["28px", {"lineHeight": "36px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                        "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}]
                    }
                }
            }
        }
    </script>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
</head>
<body class="bg-background text-on-surface font-body-md overflow-x-hidden">
<!-- Header Navigation -->
<header class="fixed top-0 w-full z-50 bg-surface/80 backdrop-blur-md border-b border-outline-variant/30">
<div class="flex items-center justify-between px-lg py-sm max-w-container-max mx-auto h-16">
<div class="flex items-center gap-sm">
<span class="material-symbols-outlined text-primary text-2xl" data-icon="terminal">terminal</span>
<span class="font-headline-md text-headline-md font-bold tracking-tight text-primary">DevPulse</span>
</div>
<nav class="hidden md:flex gap-lg items-center">
<a class="text-primary font-bold border-b-2 border-primary py-1" href="#">Profile</a>
<a class="text-on-surface-variant hover:text-primary transition-colors" href="#">Repositories</a>
<a class="text-on-surface-variant hover:text-primary transition-colors" href="#">Projects</a>
<a class="text-on-surface-variant hover:text-primary transition-colors" href="#">Insights</a>
</nav>
<div class="w-10 h-10 rounded-full border-2 border-primary/20 overflow-hidden cursor-pointer active:opacity-80 transition-all shadow-sm">
<img class="w-full h-full object-cover" data-alt="A professional studio portrait of a modern software developer smiling, wearing a sleek black hoodie, with a clean office background showing soft monitor glows and technical books. The lighting is crisp and energetic, matching a high-contrast digital professional brand aesthetic." src="https://lh3.googleusercontent.com/aida-public/AB6AXuAlG9CWrbOeqmFU36q0g0CXeg3WJ43sh7BAttcYdOuYN1OBm6MSwxRZ9GPThAjxBHmotsT-7ZkdspqXnch0PvYXQBgkXD5ylGfFO-O4T8AiYC4UpMVFDpWTej9t19s0Ark3RPH00w3JnOnbzl80UTi1w0A1AMWf49m6AkAYJ8n4xx-Uz-p3eUXlDV9e4yLQwo37JEYKSsslUFXtwh62ZNNs668HktgJ5yOXNaM-tJbHCJC0LlqoEYJJ-1af34une8Fx8yT-4VYE-qmN"/>
</div>
</div>
</header>
<main class="pt-24 pb-xl px-lg max-w-container-max mx-auto">
<!-- Hero Section -->
<section class="relative mb-xl text-center py-xl overflow-hidden rounded-xl">
<div class="absolute inset-0 z-0 opacity-10">

</div>
<div class="relative z-10 flex flex-col items-center">
<div class="w-32 h-32 md:w-40 md:h-40 rounded-full p-1 bg-gradient-to-tr from-primary via-secondary to-tertiary animate-float mb-md shadow-xl">
<div class="w-full h-full rounded-full overflow-hidden border-4 border-surface">
<img class="w-full h-full object-cover" data-alt="A high-quality 3D render of a creative developer workspace with a dual-monitor setup, mechanical keyboard with RGB lighting, and lush indoor plants. The atmosphere is vibrant and inspiring with pops of indigo and emerald green lighting against clean white walls." src="https://lh3.googleusercontent.com/aida-public/AB6AXuC6PgYtzvvfoV3Z__AyKLzMtWXLQuTnYD8eM0Ays0x1kVvnbg7cm3y_OEpDP65cyY8c9WjgUWc0P4Xj5uhSWD6ZutO3wtU1WWLq1n5QOw20a--Is50wOOzVHiPcItOhIw9111rOImwB1ACQU1Mj8Uf1955seeTMS57MB55Jeu2TtI5xducQvSPjipRVAIXMV-WIlcBPjFrcY6-KIC3azDXCd6gDceCOSBA-83sx7QnPmDSYOG-E_lmBjMmIwl36rn9CdWeVOZgivU3W"/>
</div>
</div>
<h1 class="font-headline-xl text-headline-xl text-on-surface mb-xs">
                    Hi, I'm <span class="text-primary">Alex Rivera</span> 👋
                </h1>
<p class="font-body-lg text-body-lg text-on-surface-variant max-w-2xl mb-lg">
                    Full-Stack Sorcerer &amp; Cloud Architect based in San Francisco. Building pixel-perfect experiences and scalable backends with electric precision.
                </p>
<div class="flex flex-wrap justify-center gap-md">
<button class="flex items-center gap-2 px-md py-sm rounded-lg bg-[#333] text-white hover:scale-105 transition-transform shadow-md">
<span class="material-symbols-outlined" data-icon="terminal">terminal</span> GitHub
                    </button>
<button class="flex items-center gap-2 px-md py-sm rounded-lg bg-[#0077b5] text-white hover:scale-105 transition-transform shadow-md">
<span class="material-symbols-outlined" data-icon="share">share</span> LinkedIn
                    </button>
<button class="flex items-center gap-2 px-md py-sm rounded-lg bg-[#1da1f2] text-white hover:scale-105 transition-transform shadow-md">
<span class="material-symbols-outlined" data-icon="chat">chat</span> Twitter
                    </button>
</div>
</div>
</section>
<div class="grid grid-cols-1 md:grid-cols-12 gap-lg">
<!-- Left Column: About Me -->
<div class="md:col-span-5 flex flex-col gap-lg">
<div class="bg-surface-container-lowest p-lg rounded-xl border border-outline-variant/30 shadow-sm">
<h2 class="font-headline-md text-headline-md mb-md flex items-center gap-2">
<span class="material-symbols-outlined text-tertiary" data-icon="person">person</span> About Me
                    </h2>
<ul class="space-y-md">
<li class="flex gap-md items-start">
<span class="material-symbols-outlined text-secondary p-sm rounded-lg bg-secondary-container/20" data-icon="school">school</span>
<div>
<h4 class="font-label-md text-label-md">Learning Journey</h4>
<p class="text-body-sm text-on-surface-variant">Currently mastering Web3 &amp; Distributed Systems</p>
</div>
</li>
<li class="flex gap-md items-start">
<span class="material-symbols-outlined text-primary p-sm rounded-lg bg-primary-container/20" data-icon="work">work</span>
<div>
<h4 class="font-label-md text-label-md">Current Role</h4>
<p class="text-body-sm text-on-surface-variant">Senior Engineer @ InnovateLabs</p>
</div>
</li>
<li class="flex gap-md items-start">
<span class="material-symbols-outlined text-error p-sm rounded-lg bg-error-container/20" data-icon="favorite">favorite</span>
<div>
<h4 class="font-label-md text-label-md">Passions</h4>
<p class="text-body-sm text-on-surface-variant">Open source contributor &amp; UI enthusiast</p>
</div>
</li>
</ul>
</div>
<!-- Tech Stack (Bento Style) -->
<div class="bg-surface-container-lowest p-lg rounded-xl border border-outline-variant/30 shadow-sm">
<h2 class="font-headline-md text-headline-md mb-md flex items-center gap-2">
<span class="material-symbols-outlined text-secondary" data-icon="code">code</span> Tech Stack
                    </h2>
<div class="flex flex-wrap gap-sm">
<span class="px-md py-base rounded-full bg-blue-100 text-blue-700 border border-blue-200 font-label-md flex items-center gap-1">
                            React
                        </span>
<span class="px-md py-base rounded-full bg-emerald-100 text-emerald-700 border border-emerald-200 font-label-md flex items-center gap-1">
                            Node.js
                        </span>
<span class="px-md py-base rounded-full bg-orange-100 text-orange-700 border border-orange-200 font-label-md flex items-center gap-1">
                            AWS
                        </span>
<span class="px-md py-base rounded-full bg-indigo-100 text-indigo-700 border border-indigo-200 font-label-md flex items-center gap-1">
                            TypeScript
                        </span>
<span class="px-md py-base rounded-full bg-purple-100 text-purple-700 border border-purple-200 font-label-md flex items-center gap-1">
                            GraphQL
                        </span>
<span class="px-md py-base rounded-full bg-pink-100 text-pink-700 border border-pink-200 font-label-md flex items-center gap-1">
                            Tailwind CSS
                        </span>
<span class="px-md py-base rounded-full bg-red-100 text-red-700 border border-red-200 font-label-md flex items-center gap-1">
                            Redis
                        </span>
<span class="px-md py-base rounded-full bg-cyan-100 text-cyan-700 border border-cyan-200 font-label-md flex items-center gap-1">
                            Docker
                        </span>
</div>
</div>
</div>
<!-- Right Column: Projects & GitHub Activity -->
<div class="md:col-span-7 flex flex-col gap-lg">
<h2 class="font-headline-md text-headline-md flex items-center gap-2 px-sm">
<span class="material-symbols-outlined text-primary" data-icon="star">star</span> Featured Projects
                </h2>
<div class="grid grid-cols-1 sm:grid-cols-2 gap-md">
<!-- Project Card 1 -->
<div class="group bg-surface-container-lowest rounded-xl border-l-4 border-l-primary border border-outline-variant/30 p-md hover:shadow-lg transition-all duration-300">
<div class="flex justify-between items-start mb-sm">
<span class="material-symbols-outlined text-primary-container bg-primary p-xs rounded" data-icon="rocket_launch">rocket_launch</span>
<div class="flex gap-xs">
<span class="material-symbols-outlined text-on-surface-variant text-sm" data-icon="star" style="font-variation-settings: 'FILL' 1;">star</span>
<span class="text-label-sm">1.2k</span>
</div>
</div>
<h3 class="font-label-md text-label-md mb-xs group-hover:text-primary transition-colors">PulseEngine</h3>
<p class="text-body-sm text-on-surface-variant mb-md">High-performance animation library for WebGL-based interfaces.</p>
<div class="flex items-center gap-sm">
<span class="w-3 h-3 rounded-full bg-primary"></span>
<span class="text-label-sm">TypeScript</span>
</div>
</div>
<!-- Project Card 2 -->
<div class="group bg-surface-container-lowest rounded-xl border-l-4 border-l-secondary border border-outline-variant/30 p-md hover:shadow-lg transition-all duration-300">
<div class="flex justify-between items-start mb-sm">
<span class="material-symbols-outlined text-secondary-container bg-secondary p-xs rounded" data-icon="eco">eco</span>
<div class="flex gap-xs">
<span class="material-symbols-outlined text-on-surface-variant text-sm" data-icon="star" style="font-variation-settings: 'FILL' 1;">star</span>
<span class="text-label-sm">842</span>
</div>
</div>
<h3 class="font-label-md text-label-md mb-xs group-hover:text-secondary transition-colors">LeafyStack</h3>
<p class="text-body-sm text-on-surface-variant mb-md">Carbon-neutral hosting automation for serverless deployments.</p>
<div class="flex items-center gap-sm">
<span class="w-3 h-3 rounded-full bg-secondary"></span>
<span class="text-label-sm">Rust</span>
</div>
</div>
<!-- Project Card 3 -->
<div class="group bg-surface-container-lowest rounded-xl border-l-4 border-l-tertiary border border-outline-variant/30 p-md hover:shadow-lg transition-all duration-300">
<div class="flex justify-between items-start mb-sm">
<span class="material-symbols-outlined text-tertiary-fixed bg-tertiary p-xs rounded" data-icon="database">database</span>
<div class="flex gap-xs">
<span class="material-symbols-outlined text-on-surface-variant text-sm" data-icon="star" style="font-variation-settings: 'FILL' 1;">star</span>
<span class="text-label-sm">2.4k</span>
</div>
</div>
<h3 class="font-label-md text-label-md mb-xs group-hover:text-tertiary transition-colors">SwiftDB</h3>
<p class="text-body-sm text-on-surface-variant mb-md">Key-value store optimized for low-latency edge computing.</p>
<div class="flex items-center gap-sm">
<span class="w-3 h-3 rounded-full bg-tertiary"></span>
<span class="text-label-sm">Go</span>
</div>
</div>
<!-- Project Card 4 -->
<div class="group bg-surface-container-lowest rounded-xl border-l-4 border-l-error border border-outline-variant/30 p-md hover:shadow-lg transition-all duration-300">
<div class="flex justify-between items-start mb-sm">
<span class="material-symbols-outlined text-error-container bg-error p-xs rounded" data-icon="shield">shield</span>
<div class="flex gap-xs">
<span class="material-symbols-outlined text-on-surface-variant text-sm" data-icon="star" style="font-variation-settings: 'FILL' 1;">star</span>
<span class="text-label-sm">567</span>
</div>
</div>
<h3 class="font-label-md text-label-md mb-xs group-hover:text-error transition-colors">GuardRail</h3>
<p class="text-body-sm text-on-surface-variant mb-md">Static analysis tool for catching security vulnerabilities in real-time.</p>
<div class="flex items-center gap-sm">
<span class="w-3 h-3 rounded-full bg-error"></span>
<span class="text-label-sm">Python</span>
</div>
</div>
</div>
<!-- GitHub Stats Placeholder Visualization -->
<div class="bg-surface-container-lowest rounded-xl border border-outline-variant/30 p-lg mt-sm">
<h2 class="font-headline-md text-headline-md mb-md flex items-center gap-2">
<span class="material-symbols-outlined text-primary" data-icon="analytics">analytics</span> Contribution Stats
                    </h2>
<div class="grid grid-cols-2 sm:grid-cols-4 gap-md">
<div class="text-center p-md rounded-lg bg-surface-container">
<div class="text-headline-md font-bold text-primary">524</div>
<div class="text-label-sm text-on-surface-variant">Commits</div>
</div>
<div class="text-center p-md rounded-lg bg-surface-container">
<div class="text-headline-md font-bold text-secondary">48</div>
<div class="text-label-sm text-on-surface-variant">PRs Merged</div>
</div>
<div class="text-center p-md rounded-lg bg-surface-container">
<div class="text-headline-md font-bold text-tertiary">12</div>
<div class="text-label-sm text-on-surface-variant">Projects</div>
</div>
<div class="text-center p-md rounded-lg bg-surface-container">
<div class="text-headline-md font-bold text-primary-container">1.5k</div>
<div class="text-label-sm text-on-surface-variant">Followers</div>
</div>
</div>
</div>
</div>
</div>
<!-- CTA Section -->
<section class="mt-xl text-center py-xl relative">
<div class="absolute inset-0 z-0 bg-primary/5 rounded-3xl -rotate-1"></div>
<div class="relative z-10 flex flex-col items-center">
<h2 class="font-headline-lg text-headline-lg mb-sm">Let's build something extraordinary</h2>
<p class="text-body-lg text-on-surface-variant mb-lg max-w-xl">
                    I'm currently open to freelance opportunities and technical collaborations. If you have an exciting project in mind, let's talk.
                </p>
<a class="vibrant-gradient text-white px-xl py-md rounded-full font-headline-md shadow-lg shadow-primary/30 hover:scale-105 active:scale-95 transition-all flex items-center gap-md" href="mailto:hello@devpulse.com">
                    Get in touch <span class="material-symbols-outlined" data-icon="send">send</span>
</a>
</div>
</section>
</main>
<footer class="w-full py-xl bg-surface-container-lowest border-t border-outline-variant/50 mt-xl">
<div class="flex flex-col md:flex-row items-center justify-between px-lg max-w-container-max mx-auto gap-md">
<div class="flex items-center gap-sm">
<span class="material-symbols-outlined text-primary text-xl" data-icon="terminal">terminal</span>
<span class="font-label-md text-label-md font-semibold text-on-surface">© 2024 DevPulse. Crafted for the modern web.</span>
</div>
<div class="flex gap-lg">
<a class="text-on-surface-variant hover:text-tertiary transition-all underline underline-offset-4 font-body-sm" href="#">GitHub</a>
<a class="text-on-surface-variant hover:text-tertiary transition-all underline underline-offset-4 font-body-sm" href="#">LinkedIn</a>
<a class="text-on-surface-variant hover:text-tertiary transition-all underline underline-offset-4 font-body-sm" href="#">Twitter</a>
<a class="text-on-surface-variant hover:text-tertiary transition-all underline underline-offset-4 font-body-sm" href="#">Portfolio</a>
</div>
</div>
</footer>
<script>
        // Simple micro-interaction for cards
        document.querySelectorAll('.group').forEach(card => {
            card.addEventListener('mouseenter', () => {
                const icon = card.querySelector('.material-symbols-outlined');
                if(icon) icon.style.transform = 'scale(1.1) rotate(5deg)';
            });
            card.addEventListener('mouseleave', () => {
                const icon = card.querySelector('.material-symbols-outlined');
                if(icon) icon.style.transform = 'scale(1) rotate(0deg)';
            });
        });

        // Sticky header opacity change on scroll
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 20) {
                header.classList.add('shadow-md');
                header.classList.remove('bg-surface/80');
                header.classList.add('bg-surface/95');
            } else {
                header.classList.remove('shadow-md');
                header.classList.remove('bg-surface/95');
                header.classList.add('bg-surface/80');
            }
        });
    </script>
</body></html>
