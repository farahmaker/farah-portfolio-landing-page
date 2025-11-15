# farah-portfolio-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Farah | Aspiring Web Developer & Intern</title>
    
    <!-- Load Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Configure Tailwind for custom colors and use Inter font -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary-red': '#E53E3E', // Primary Red Accent
                        'secondary-gray': '#F7FAFC', // Off-white for section backgrounds
                        'accent-dark': '#1A202C', // Dark text for strong contrast
                        'light-bg': '#FFFFFF', // Pure white background
                        'text-color': '#4A5568', // Standard text color
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    
    <!-- Custom style for the Inter font and smooth transitions -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #FFFFFF;
            color: #4A5566;
        }
        .card-hover:hover {
            transform: translateY(-4px);
            box-shadow: 0 15px 30px rgba(229, 62, 62, 0.1);
        }
        /* Mobile adjustment for better spacing */
        @media (max-width: 640px) {
            .section-padding {
                padding-top: 3rem;
                padding-bottom: 3rem;
            }
        }
    </style>
</head>
<body class="min-h-screen antialiased">

    <!-- Header (Simple & Focused Navigation) -->
    <header class="bg-light-bg shadow-md sticky top-0 z-10 border-b border-gray-100">
        <div class="max-w-5xl mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-extrabold text-accent-dark">FARAH</h1>
            <!-- Only primary CTAs in navigation for a clean look -->
            <a href="#contact" class="text-sm font-semibold text-light-bg bg-primary-red py-2 px-5 rounded-full hover:bg-red-700 transition duration-300 shadow-md">
                Get in Touch
            </a>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="max-w-5xl mx-auto px-4">

        <!-- 1. HERO SECTION: The Core Message (About/Objective) -->
        <section id="hero" class="text-center section-padding pt-20 pb-16 sm:pt-32 sm:pb-24">
            <div class="mx-auto w-24 h-24 bg-primary-red rounded-full mb-6 flex items-center justify-center text-4xl text-light-bg font-bold shadow-xl">F</div>
            
            <h2 class="text-4xl sm:text-5xl font-extrabold mb-4 text-accent-dark leading-tight">
                Self-Taught & Determined <span class="text-primary-red">Web Development Intern</span>
            </h2>
            
            <p class="text-xl text-text-color max-w-3xl mx-auto mb-8">
                I'm Farah, an Honors student with a strong drive to transition into tech. Despite a non-technical background, I’ve independently mastered **HTML, CSS, and basic JavaScript**. I seek an internship to apply my foundational skills and dedication to a real-world project environment.
            </p>
            
            <!-- Primary Call to Action -->
            <div class="mt-8 space-x-4">
                <a href="#projects" class="inline-block bg-primary-red text-light-bg font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-red-700 transition duration-300 transform hover:scale-105">
                    View Portfolio Project
                </a>
                <a href="mailto:asrafi.farah@gmail.com" class="inline-block text-primary-red border-2 border-primary-red font-semibold py-3 px-8 rounded-full hover:bg-red-50 transition duration-300">
                    Email Me (asrafi.farah@gmail.com)
                </a>
            </div>
        </section>

        <!-- Separator for visual interest -->
        <div class="h-1 bg-gray-100 max-w-2xl mx-auto rounded-full"></div>

        <!-- 2. SKILLS SECTION: What I Bring -->
        <section id="skills" class="section-padding py-16">
            <h3 class="text-3xl font-bold text-center text-accent-dark mb-10">Foundational Knowledge</h3>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-8">
                
                <!-- Skill Card 1: HTML & Structure -->
                <div class="bg-secondary-gray p-6 rounded-xl text-center shadow-lg card-hover transition duration-300 border-b-4 border-primary-red">
                    <p class="text-4xl mb-3">🏷️</p>
                    <p class="font-bold text-lg text-accent-dark">HTML Structure</p>
                    <p class="text-sm text-text-color mt-1">Semantic structuring and accessibility basics.</p>
                </div>
                
                <!-- Skill Card 2: CSS & Layout -->
                <div class="bg-secondary-gray p-6 rounded-xl text-center shadow-lg card-hover transition duration-300 border-b-4 border-primary-red">
                    <p class="text-4xl mb-3">🎨</p>
                    <p class="font-bold text-lg text-accent-dark">CSS & Responsive Layouts</p>
                    <p class="text-sm text-text-color mt-1">Mastery of Flexbox/Grid for mobile-first design.</p>
                </div>
                
                <!-- Skill Card 3: JavaScript -->
                <div class="bg-secondary-gray p-6 rounded-xl text-center shadow-lg card-hover transition duration-300 border-b-4 border-primary-red">
                    <p class="text-4xl mb-3">💻</p>
                    <p class="font-bold text-lg text-accent-dark">JavaScript Basics</p>
                    <p class="text-sm text-text-color mt-1">Variables, functions, DOM manipulation fundamentals.</p>
                </div>
                
                <!-- Skill Card 4: Backend Exploration -->
                <div class="bg-secondary-gray p-6 rounded-xl text-center shadow-lg card-hover transition duration-300 border-b-4 border-primary-red">
                    <p class="text-4xl mb-3">💡</p>
                    <p class="font-bold text-lg text-accent-dark">Backend Concepts</p>
                    <p class="text-sm text-text-color mt-1">Exposure to Python, C++, and SQL concepts.</p>
                </div>
            </div>
        </section>

        <!-- 3. PROJECT SECTION: Proof of Work -->
        <section id="projects" class="section-padding py-16 bg-secondary-gray rounded-xl shadow-inner mb-16">
            <h3 class="text-3xl font-bold text-center text-accent-dark mb-10">My Proof of Initiative</h3>
            
            <!-- Project Card -->
            <div class="max-w-3xl mx-auto bg-light-bg p-8 rounded-xl shadow-2xl border-l-8 border-primary-red transition duration-300">
                <h4 class="text-2xl font-bold mb-2 text-accent-dark">Static Portfolio Website</h4>
                <p class="text-lg text-text-color mb-4">
                    **Core Achievement:** Independently planned and executed a static portfolio to immediately translate theoretical HTML/CSS knowledge into a tangible, live project.
                </p>
                <ul class="list-disc list-inside text-gray-600 space-y-1 ml-4">
                    <li>Focus on clean, modern layout design using **Tailwind CSS (utility-first approach)**.</li>
                    <li>Ensured the page is **fully responsive** and optimized for mobile viewing.</li>
                    <li>Demonstrated ability to follow a specific design constraint (White & Red theme).</li>
                </ul>
                <!-- Note: In a real app, this link would go to the hosted project -->
                <div class="mt-6 text-center">
                    <span class="inline-block bg-primary-red text-light-bg font-semibold py-2 px-6 rounded-full opacity-75">
                        [Project Link Placeholder]
                    </span>
                </div>
            </div>
            
            <p class="text-center text-text-color italic mt-8">
                Future projects will focus on adding interactive features using **JavaScript** and integrating **Python/SQL** for the backend.
            </p>
        </section>

        <!-- 4. CONTACT SECTION: Final CTA -->
        <section id="contact" class="section-padding pt-8 pb-20 text-center">
            <h3 class="text-3xl font-bold text-accent-dark mb-4">Ready to Start Contributing.</h3>
            <p class="text-lg text-text-color max-w-3xl mx-auto mb-8">
                I am actively seeking an internship opportunity where I can work hard, learn fast, and grow into a professional Web Developer. My drive and foundation are ready to be tested and utilized.
            </p>
            
            <a href="mailto:asrafi.farah@gmail.com" class="inline-block bg-primary-red text-light-bg font-extrabold text-xl py-4 px-12 rounded-full shadow-2xl hover:bg-red-700 transition duration-300 transform hover:scale-105">
                Apply My Dedication Here →
            </a>
            <p class="text-sm text-gray-500 mt-4">asrafi.farah@gmail.com</p>
        </section>
        
    </main>

    <!-- Footer -->
    <footer class="bg-secondary-gray border-t border-gray-200 mt-12 py-6">
        <div class="max-w-5xl mx-auto px-4 text-center">
            <p class="text-sm text-gray-500">&copy; Farah - Aspiring Developer | Built with HTML & Tailwind CSS.</p>
        </div>
    </footer>

</body>
</html>
