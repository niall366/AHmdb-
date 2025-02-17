<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AHmdb: Ratings & Reviews</title>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: #fff;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: space-between;
        }

        /* Header */
        header {
            background-color: #333;
            padding: 20px;
            width: 100%;
            text-align: center;
        }

        header h1 {
            font-size: 3em;
            color: #f39c12;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }

        /* Search bar */
        #search-bar {
            margin-top: 10px;
            padding: 10px;
            width: 80%;
            font-size: 1.2em;
            border-radius: 5px;
            border: none;
        }

        /* Sidebar menu */
        #sidebar {
            width: 200px;
            background-color: #222;
            padding-top: 20px;
            position: fixed;
            height: 100vh;
            top: 0;
        }

        #sidebar a {
            color: #fff;
            text-decoration: none;
            display: block;
            margin: 10px 0;
            padding: 10px;
            font-size: 1.2em;
        }

        #sidebar a:hover {
            background-color: #f39c12;
        }

        /* Content Area */
        #content {
            margin-left: 220px;
            padding: 20px;
            width: calc(100% - 220px);
        }

        /* Movie sections */
        #rated, #unrated, #funfacts, #quizzes {
            display: none;
            margin: 20px;
        }

        .movie {
            background-color: #333;
            margin: 10px 0;
            padding: 15px;
            border-radius: 10px;
        }

        /* Fun Facts */
        .fun-fact {
            background-color: #444;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
        }

        .editor-sticker {
            background-color: #e74c3c;
            color: white;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            position: absolute;
            top: 10px;
            left: 10px;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        /* Quote Section */
        .quote-section {
            background-color: #444;
            padding: 20px;
            margin: 20px 0;
            border-radius: 10px;
            font-style: italic;
        }

        /* Quiz Section */
        .quiz-container {
            background-color: #444;
            padding: 15px;
            border-radius: 10px;
            margin: 10px 0;
        }

        .quiz-question {
            font-size: 1.2em;
        }

        .quiz-answer {
            margin: 10px 0;
        }

    </style>
</head>
<body>
    <!-- Sidebar -->
    <div id="sidebar">
        <a href="javascript:void(0)" class="menu-button" onclick="toggleSection('rated')">Rated Movies</a>
        <a href="javascript:void(0)" class="menu-button" onclick="toggleSection('unrated')">Unrated Movies</a>
        <a href="javascript:void(0)" class="menu-button" onclick="toggleSection('funfacts')">Movie Fun Facts</a>
        <a href="javascript:void(0)" class="menu-button" onclick="toggleSection('quizzes')">Quizzes</a>
    </div>

    <!-- Main Content -->
    <div id="content">
        <header>
            <h1>AHmdb: Ratings & Reviews</h1>
            <input type="text" id="search-bar" placeholder="Search for movies...">
        </header>

        <!-- Fun Facts Section -->
        <div id="funfacts" class="section">
            <h2>Fun Facts</h2>
            <div class="fun-fact">
                <h4>Batman Trivia</h4>
                <p>Batman’s first appearance was in Detective Comics #27 in 1939.</p>
                <img src="batman_image.jpg" alt="Batman" width="300">
            </div>
            <div class="fun-fact">
                <h4>Gladiator Trivia</h4>
                <p>Russell Crowe had to train for months to prepare for his role in Gladiator, including sword-fighting and horseback riding.</p>
                <img src="gladiator_image.jpg" alt="Gladiator" width="300">
            </div>
        </div>

        <!-- Rated Movies -->
        <div id="rated" class="section">
            <h2>Rated Movies</h2>
            <!-- Rated Movies List -->
            <div class="movie">
                <div class="editor-sticker">Editor's Pick</div>
                <h3>Batman</h3>
                <p>Rating: <span class="stars">★★★★☆</span></p>
                <p>Description: A brief description about Batman movie.</p>
            </div>
            <div class="movie">
                <h3>Gladiator</h3>
                <p>Rating: <span class="stars">★★★★★</span></p>
                <p>Description: A brief description about Gladiator movie.</p>
            </div>
        </div>

        <!-- Unrated Movies -->
        <div id="unrated" class="section">
            <h2>Unrated Movies</h2>
            <!-- Unrated Movies List -->
            <div class="movie">
                <h3>Inception</h3>
                <p>Description: A mind-bending thriller about dreams.</p>
                <button onclick="rateMovie(this, 'rated')">Rate this Movie</button>
            </div>
            <div class="movie">
                <h3>Interstellar</h3>
                <p>Description: A journey through space and time.</p>
                <button onclick="rateMovie(this, 'rated')">Rate this Movie</button>
            </div>
            <!-- More unrated movies would follow... -->
        </div>

        <!-- Quote Section -->
        <div class="quote-section">
            <p>“You know, you remind me of my father. I hated my father! He was a drinker, and a fiend. And one night, he goes off crazier than usual. Mommy gets the kitchen knife to defend herself. He doesn't like that. Not. One. Bit. So, me watching, he takes the knife to her, laughing while he does it. He turns to me, and he says, 'Why so serious, son?' Comes at me with the knife—'Why so serious, son?' He sticks the blade in my mouth—'Let's put a smile on that face!' And… why so serious?”</p>
            <p>- Joker</p>
        </div>

        <!-- Quizzes Section -->
        <div id="quizzes" class="section">
            <h2>Movie Quizzes</h2>
            <div class="quiz-container">
                <div class="quiz-question">
                    <h4>Which actor played the role of the Joker in "The Dark Knight"?</h4>
                </div>
                <div class="quiz-answer">
                    <input type="radio" id="heath" name="joker" value="Heath Ledger">
                    <label for="heath">Heath Ledger</label>
                </div>
                <div class="quiz-answer">
                    <input type="radio" id="jack" name="joker" value="Jack Nicholson">
                    <label for="jack">Jack Nicholson</label>
                </div>
                <div class="quiz-answer">
                    <input type="radio" id="jared" name="joker" value="Jared Leto">
                    <label for="jared">Jared Leto</label>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <footer>
            <p>AHmdb: Our Movie Database</p>
            <p>Our Team: Anela & Hamza</p>
            <p>Located: Visoko & Tešanj, BiH</p>
        </footer>
    </div>

    <script>
        function toggleSection(section) {
            // Hide all sections
            document.getElementById('rated').classList.remove('show');
            document.getElementById('unrated').classList.remove('show');
            document.getElementById('funfacts').classList.remove('show');
            document.getElementById('quizzes').classList.remove('show');

            // Show the selected section
            document.getElementById(section).classList.add('show');
        }

        function rateMovie(button, section) {
            // Move unrated movie to rated section after clicking rate
            const movie = button.parentElement;
            document.getElementById(section).appendChild(movie);
            button.disabled = true;  // Disable button after rating
            button.innerText = "Rated!";
        }
    </script>
</body>
</html>
