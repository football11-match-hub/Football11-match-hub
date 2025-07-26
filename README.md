<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Football Match Hub</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f2f5; /* Light gray background */
        }
        .match-card {
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
            transition: transform 0.2s ease-in-out;
        }
        .match-card:hover {
            transform: translateY(-5px);
        }
        .team-logo {
            width: 60px;
            height: 60px;
            object-fit: contain;
            border-radius: 8px;
        }
        .live-indicator {
            animation: pulse 1.5s infinite;
        }
        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.05); opacity: 0.7; }
            100% { transform: scale(1); opacity: 1; }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">
    <div class="container mx-auto p-4 sm:p-6 lg:p-8">
        <!-- Header -->
        <header class="bg-gradient-to-r from-blue-600 to-indigo-700 text-white p-6 rounded-xl shadow-lg mb-8">
            <h1 class="text-3xl sm:text-4xl font-extrabold text-center mb-2">Football Match Hub</h1>
            <p class="text-center text-lg sm:text-xl font-light">Your ultimate source for live scores, fixtures, and news!</p>
        </header>

        <!-- Live Matches Section -->
        <section class="mb-10">
            <h2 class="text-2xl sm:text-3xl font-bold text-gray-900 mb-6 text-center">⚽ Live Matches</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Live Match Card 1 -->
                <div class="match-card p-6 flex flex-col items-center justify-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/0000FF/FFFFFF?text=CHE" alt="Chelsea Logo" class="team-logo mr-4">
                        <span class="text-3xl font-bold text-blue-700">2</span>
                        <span class="text-2xl font-semibold mx-4">-</span>
                        <span class="text-3xl font-bold text-red-700">1</span>
                        <img src="https://placehold.co/60x60/FF0000/FFFFFF?text=LIV" alt="Liverpool Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">Chelsea vs Liverpool</p>
                    <div class="flex items-center text-green-600 font-bold mb-4">
                        <span class="relative flex h-3 w-3 mr-2">
                            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
                            <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
                        </span>
                        Live <span class="ml-2 text-sm font-normal text-gray-500">(85')</span>
                    </div>
                    <p class="text-sm text-gray-500">Premier League</p>
                </div>

                <!-- Live Match Card 2 -->
                <div class="match-card p-6 flex flex-col items-center justify-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/FFD700/000000?text=MUN" alt="Man Utd Logo" class="team-logo mr-4">
                        <span class="text-3xl font-bold text-yellow-600">0</span>
                        <span class="text-2xl font-semibold mx-4">-</span>
                        <span class="text-3xl font-bold text-purple-700">0</span>
                        <img src="https://placehold.co/60x60/800080/FFFFFF?text=ARS" alt="Arsenal Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">Man Utd vs Arsenal</p>
                    <div class="flex items-center text-green-600 font-bold mb-4">
                        <span class="relative flex h-3 w-3 mr-2">
                            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
                            <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
                        </span>
                        Live <span class="ml-2 text-sm font-normal text-gray-500">(Half-time)</span>
                    </div>
                    <p class="text-sm text-gray-500">Premier League</p>
                </div>

                <!-- Live Match Card 3 -->
                <div class="match-card p-6 flex flex-col items-center justify-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/FF4500/FFFFFF?text=BAR" alt="Barcelona Logo" class="team-logo mr-4">
                        <span class="text-3xl font-bold text-orange-600">3</span>
                        <span class="text-2xl font-semibold mx-4">-</span>
                        <span class="text-3xl font-bold text-gray-700">0</span>
                        <img src="https://placehold.co/60x60/808080/FFFFFF?text=RMA" alt="Real Madrid Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">Barcelona vs Real Madrid</p>
                    <div class="flex items-center text-green-600 font-bold mb-4">
                        <span class="relative flex h-3 w-3 mr-2">
                            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
                            <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
                        </span>
                        Live <span class="ml-2 text-sm font-normal text-gray-500">(60')</span>
                    </div>
                    <p class="text-sm text-gray-500">La Liga</p>
                </div>
            </div>
        </section>

        <!-- Upcoming Matches Section -->
        <section class="mb-10">
            <h2 class="text-2xl sm:text-3xl font-bold text-gray-900 mb-6 text-center">🗓️ Upcoming Matches</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Upcoming Match Card 1 -->
                <div class="match-card p-6 flex flex-col items-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/008000/FFFFFF?text=MCI" alt="Man City Logo" class="team-logo mr-4">
                        <span class="text-2xl font-semibold mx-4">vs</span>
                        <img src="https://placehold.co/60x60/8B0000/FFFFFF?text=TOT" alt="Tottenham Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">Man City vs Tottenham</p>
                    <p class="text-md text-gray-600 mb-2">Tomorrow, 10:00 PM IST</p>
                    <p class="text-sm text-gray-500">Premier League</p>
                </div>

                <!-- Upcoming Match Card 2 -->
                <div class="match-card p-6 flex flex-col items-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/A52A2A/FFFFFF?text=JUV" alt="Juventus Logo" class="team-logo mr-4">
                        <span class="text-2xl font-semibold mx-4">vs</span>
                        <img src="https://placehold.co/60x60/000000/FFFFFF?text=INT" alt="Inter Milan Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">Juventus vs Inter Milan</p>
                    <p class="text-md text-gray-600 mb-2">Sunday, 12:30 AM IST</p>
                    <p class="text-sm text-gray-500">Serie A</p>
                </div>

                <!-- Upcoming Match Card 3 -->
                <div class="match-card p-6 flex flex-col items-center text-center">
                    <div class="flex items-center justify-center w-full mb-4">
                        <img src="https://placehold.co/60x60/FFC0CB/000000?text=PSG" alt="PSG Logo" class="team-logo mr-4">
                        <span class="text-2xl font-semibold mx-4">vs</span>
                        <img src="https://placehold.co/60x60/800000/FFFFFF?text=MAR" alt="Marseille Logo" class="team-logo ml-4">
                    </div>
                    <p class="text-xl font-semibold mb-2">PSG vs Marseille</p>
                    <p class="text-md text-gray-600 mb-2">Sunday, 01:00 AM IST</p>
                    <p class="text-sm text-gray-500">Ligue 1</p>
                </div>
            </div>
        </section>

        <!-- News Section -->
        <section class="mb-10">
            <h2 class="text-2xl sm:text-3xl font-bold text-gray-900 mb-6 text-center">📰 Latest News</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- News Card 1 -->
                <div class="match-card p-6">
                    <h3 class="text-xl font-semibold mb-2">Mbappe's Future: Real Madrid or PSG?</h3>
                    <p class="text-gray-700 text-sm mb-4">Speculation continues to mount over Kylian Mbappe's next move as his contract situation remains unresolved. Fans eagerly await an announcement.</p>
                    <a href="#" class="text-blue-600 hover:underline text-sm font-medium">Read More →</a>
                </div>
                <!-- News Card 2 -->
                <div class="match-card p-6">
                    <h3 class="text-xl font-semibold mb-2">Premier League Title Race Heats Up!</h3>
                    <p class="text-gray-700 text-sm mb-4">With only a few games left, the top three teams are neck and neck in the most thrilling Premier League title race in years.</p>
                    <a href="#" class="text-blue-600 hover:underline text-sm font-medium">Read More →</a>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="text-center text-gray-600 text-sm mt-10 p-4 border-t border-gray-200">
            © 2025 Football Match Hub. All rights reserved.
        </footer>
    </div>
</body>
</html>


