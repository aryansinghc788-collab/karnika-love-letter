<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>💌 For My Beautiful Karnika (Arka) 💖</title>
    
    <style>
        /* Base Styles */
        body {
            font-family: 'Georgia', serif;
            margin: 0;
            padding: 0;
            background-color: #ffe0e6;
            color: #4a001a;
            line-height: 1.6;
            overflow: hidden; 
        }

        /* Container for Slides */
        #slides-container {
            width: 100vw;
            height: 100vh;
            display: flex;
            transition: transform 0.6s ease-in-out; 
        }

        /* Individual Slide Styles */
        .slide {
            flex-shrink: 0;
            width: 100vw;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
            box-sizing: border-box;
            cursor: pointer; 
            position: relative; 
        }

        .slide-content {
            max-width: 85%;
            background-color: #ffffff;
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
            opacity: 0; 
            transform: scale(0.9); 
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
            position: relative;
            z-index: 10; 
        }

        /* Active Slide Styling */
        .slide.active .slide-content {
            opacity: 1; 
            transform: scale(1); 
        }

        /* --- HEART SHOWER EFFECT STYLES --- */
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff3366;
            transform: rotate(-45deg);
            z-index: 5;
            pointer-events: none;
            animation: fall linear infinite;
        }

        .heart::before, .heart::after {
            content: "";
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff3366;
            border-radius: 50%;
        }

        .heart::before {
            top: -50%;
            left: 0;
        }

        .heart::after {
            top: 0;
            left: 50%;
        }

        @keyframes fall {
            to {
                transform: translateY(100vh) rotate(200deg);
                opacity: 0;
            }
        }
        /* --- END HEART SHOWER STYLES --- */

        /* Slide-specific Styling */
        #slide-1 { background-color: #ffcccc; } 
        #slide-2 { background-color: #ff99aa; } 
        #slide-3 { background-color: #f0c3d5; }
        #slide-4 { background-color: #ff5c8a; color: white; } 
        #slide-5 { background-color: #cc6688; color: white; } 
        #slide-6 { background-color: #a879a8; color: white; } 
        #slide-7 { background-color: #e0f2f1; color: #4a001a; }
        #slide-8 { background-color: #fce4ec; } 
        
        /* Typography */
        h1 {
            color: inherit; 
            font-size: 2.5em;
            margin-bottom: 10px;
            border-bottom: 2px solid;
            padding-bottom: 5px;
        }
        
        .thought-body {
            font-size: 1.2em;
            margin-top: 20px;
            white-space: pre-wrap; 
            color: inherit;
        }
        
        /* Specific style for Shayari */
        .shayari-text {
            font-size: 1.4em;
            font-style: italic;
            margin: 25px 0;
            line-height: 1.8;
            font-family: 'Times New Roman', serif;
            color: white;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }
        
        footer {
            margin-top: 40px;
            font-size: 1.1em;
            font-weight: bold;
            color: #ff3366;
        }

        /* Call to Action Pulse Animation */
        .call-to-action {
            margin-top: 30px;
            font-size: 1em;
            color: #ff3366;
            font-weight: bold;
            animation: pulse 1.5s infinite alternate;
        }

        @keyframes pulse {
            from { transform: scale(1); opacity: 1; }
            to { transform: scale(1.05); opacity: 0.7; }
        }
        
        /* Desktop Adjustment for comfort */
        @media (min-width: 768px) {
            .slide-content {
                max-width: 700px;
            }
        }

    </style>
</head>
<body>

    <div id="slides-container">

        <div class="slide active" id="slide-1" onclick="nextSlide()">
            <div class="slide-content">
                <h1 style="color: #ff3366;">A Private Journey for Karnika (My Arka)</h1>
                <div class="thought-body">
                    <p>
                        My dearest, I’ve collected all those running thoughts in my head and put them here,
                        just for your eyes. Each tap takes you deeper into my heart.
                        This is my happy place, and you are the reason for it.
                    </p>
                </div>
                <p class="call-to-action">Tap anywhere to see my first thought 👆</p>
            </div>
        </div>

        <div class="slide" id="slide-2" onclick="nextSlide()">
            <div class="slide-content">
                <h1 style="color: #cc0033;">The Pure Comfort of You</h1>
                <div class="thought-body">
                    <p>
                        There's a quiet, deep comfort I feel whenever you're near.
                        It’s like coming home after a long journey—suddenly, all the noise stops,
                        and the world makes perfect sense. Thank you for being my peace.
                    </p>
                </div>
                <p class="call-to-action">Tap to continue the journey...</p>
            </div>
        </div>

        <div class="slide" id="slide-3" onclick="nextSlide()">
            <div class="slide-content">
                <h1 style="color: #ff007f;">Building Our Story Together</h1>
                <div class="thought-body">
                    <p>
                        I love talking about the future with you. Not just big plans, but the little things—
                        the quiet weekends, the silly arguments over movies, the shared laughter.
                        Every day with you feels like adding a beautiful, essential chapter to our book.
                    </p>
                </div>
                <p class="call-to-action">Tap for a special sentiment...</p>
            </div>
        </div>

        <div class="slide" id="slide-4" onclick="nextSlide()">
            <div class="slide-content" style="background-color: #a04000; color: white;">
                <h1 style="color: white;">Tumhari Aankhon Mein...</h1>
                <div class="thought-body">
                    <p class="shayari-text">
                        "Teri aankhon mein woh nasha hai,<br>
                        Jo mere hosh udane ko kaafi hai.<br>
                        Tu bas saamne baith ja, Arka,<br>
                        Yeh ishq ka manzar dekhne ko kaafi hai."
                    </p>
                    <p style="font-size: 1em; margin-top: 30px; font-style: italic;">
                        (There is that intoxication in your eyes,<br>
                        which is enough to make me lose myself.<br>
                        Just sit in front of me, Arka,<br>
                        This view of love is enough to last a lifetime.)
                    </p>
                </div>
                <p class="call-to-action" style="color: #ffd700;">Tap for the next deep thought...</p>
            </div>
        </div>

        <div class="slide" id="slide-5" onclick="nextSlide()">
            <div class="slide-content" style="background-color: #cc6688; color: white;">
                <h1 style="color: white; border-bottom: 2px solid white;">The Unstoppable Arka</h1>
                <div class="thought-body">
                    <p style="color: white;">
                        I am constantly in awe of your ambition and resilience. When you set your mind
                        to something, the entire world seems to move aside for you. I don't just love
                        you; I admire the amazing, powerful woman you are becoming. Never stop shining.
                    </p>
                </div>
                <p class="call-to-action" style="color: #ffddaa;">Tap to feel the love...</p>
            </div>
        </div>

        <div class="slide" id="slide-6" onclick="nextSlide()">
            <div class="slide-content" style="background-color: #a879a8; color: white;">
                <h1 style="color: white; border-bottom: 2px solid white;">Sirf Tum Hi Ho...</h1>
                <div class="thought-body">
                    <p class="shayari-text" style="font-size: 1.3em;">
                        "Har pal meri zindagi ki chahat ban gayi ho tum,<br>
                        Meri sukoon, meri rahat, meri ibadat ban gayi ho tum.<br>
                        Mil jaati hai har khushi jab tum saath hoti ho,<br>
                        Meri har dua ka jawab aur aakhri mannat ban gayi ho tum."
                    </p>
                    <p class="shayari-text" style="font-size: 1.3em; margin-top: 30px;">
                        "Dil ka sukoon, rooh ka aaram ho tum.<br>
                        Meri bandagi ka behtareen inaam ho tum."
                    </p>
                </div>
                <p class="call-to-action" style="color: #ffddaa;">Tap for the final deep thought! ✨</p>
            </div>
        </div>

        <div class="slide" id="slide-7" onclick="nextSlide()">
            <div class="slide-content">
                <h1 style="color: #00897b;">The Joy in the Ordinary</h1>
                <div class="thought-body">
                    <p>
                        It's the mundane moments I treasure most: cooking together, silently working in the same room,
                        or just grabbing your hand for no reason. These little, effortless moments confirm
                        that loving you is the easiest, most natural thing I have ever done.
                    </p>
                </div>
                <p class="call-to-action">Tap for the final message...</p>
            </div>
        </div>

        <div class="slide" id="slide-8" onclick="endSlides()">
            <div class="slide-content">
                <h1 style="color: #ff3366;">A Promise to My Love</h1>
                <div class="thought-body">
                    <p>
                        My promise to you, my beautiful Karnika (Arka), is a lifetime of unwavering support.
                        I promise to be your safe harbor, your honest critic when you need it, and your loudest
                        cheerleader, always. Thank you for making my life full.
                    </p>
                </div>
                <footer>
                    <p>I love you with all my heart.<br>— Your Boyfriend, Forever and Always.</p>
                </footer>
            </div>
        </div>

    </div>

    <script>
        let currentSlide = 0;
        const slidesContainer = document.getElementById('slides-container');
        const slides = document.querySelectorAll('.slide');
        const totalSlides = slides.length;

        // Function to start the heart shower
        function startHeartShower() {
            const slide = slides[currentSlide];
            // Clear existing hearts from this slide before adding new ones
            slide.querySelectorAll('.heart').forEach(h => h.remove());

            for (let i = 0; i < 30; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                const size = Math.random() * 15 + 10;
                heart.style.left = `${Math.random() * 100}vw`;
                heart.style.width = `${size}px`;
                heart.style.height = `${size}px`;
                heart.style.animationDelay = `${Math.random() * 3}s`;
                heart.style.animationDuration = `${Math.random() * 5 + 5}s`;
                heart.style.top = `-${size}px`; 
                slide.appendChild(heart);
            }
        }

        // Main function to move to the next slide
        function nextSlide() {
            if (currentSlide < totalSlides - 1) {
                slides[currentSlide].classList.remove('active');
                currentSlide++;
                
                slidesContainer.style.transform = `translateX(-${currentSlide * 100}vw)`;
                slides[currentSlide].classList.add('active');

                // *** CRITICAL CHANGE HERE: Call startHeartShower() on every slide after the first ***
                // The delay ensures the slide transition animation plays first.
                setTimeout(startHeartShower, 600); 
            }
        }
        
        // Function called on the very last slide click
        function endSlides() {
             // You can add a final alert or simply do nothing so the final message stays on screen.
             // The heart shower will continue on this slide.
        }

        // Initialize the first slide animation on load 
        document.addEventListener('DOMContentLoaded', () => {
             setTimeout(() => {
                slides[currentSlide].classList.add('active');
             }, 50); 
             // Optionally start hearts on the very first slide too, if desired
             // setTimeout(startHeartShower, 700); 
        });

    </script>
</body>
</html>
