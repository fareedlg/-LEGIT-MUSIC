# -LEGIT-MUSIC
Music, beautifully simple
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MyMusic - Stream & Download Music</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <i class="fas fa-headphones"></i>
                <span>MyMusic</span>
            </div>
            <div class="search-bar">
                <i class="fas fa-search"></i>
                <input type="text" placeholder="Search for artists, songs, or albums...">
            </div>
            <div class="nav-links">
                <button class="upload-btn"><i class="fas fa-upload"></i> Upload</button>
                <button class="login-btn">Sign In</button>
                <div class="user-avatar">
                    <i class="fas fa-user-circle"></i>
                </div>
            </div>
        </div>
    </nav>

    <!-- Main Container -->
    <div class="main-container">
        <!-- Sidebar -->
        <aside class="sidebar">
            <div class="sidebar-nav">
                <a href="#" class="active"><i class="fas fa-home"></i> Home</a>
                <a href="#"><i class="fas fa-fire"></i> Trending</a>
                <a href="#"><i class="fas fa-compass"></i> Explore</a>
                <a href="#"><i class="fas fa-chart-line"></i> Charts</a>
            </div>
            
            <div class="sidebar-section">
                <h3>Your Library</h3>
                <a href="#"><i class="fas fa-clock"></i> Recently Played</a>
                <a href="#"><i class="fas fa-heart"></i> Liked Songs</a>
                <a href="#"><i class="fas fa-list"></i> Playlists</a>
                <a href="#"><i class="fas fa-folder"></i> Albums</a>
            </div>
            
            <div class="sidebar-playlists">
                <h3>Your Playlists</h3>
                <a href="#">🎵 Chill Vibes</a>
                <a href="#">🔥 Workout Mix</a>
                <a href="#">💤 Sleep Sounds</a>
                <a href="#">🎉 Party Hits 2024</a>
            </div>
        </aside>

        <!-- Main Content -->
        <main class="content">
            <!-- Hero Section -->
            <section class="hero">
                <div class="hero-content">
                    <h1>Discover New Music</h1>
                    <p>Stream unlimited music, discover trending tracks, and create your perfect playlist</p>
                    <button class="cta-btn">Start Listening Now</button>
                </div>
            </section>

            <!-- Trending Section -->
            <section class="trending-section">
                <div class="section-header">
                    <h2>🔥 Trending Now</h2>
                    <a href="#">View All</a>
                </div>
                <div class="song-grid" id="trendingGrid">
                    <!-- Songs will be populated by JavaScript -->
                </div>
            </section>

            <!-- New Releases -->
            <section class="new-releases">
                <div class="section-header">
                    <h2>🆕 New Releases</h2>
                    <a href="#">View All</a>
                </div>
                <div class="album-grid" id="newReleasesGrid">
                    <!-- Albums will be populated by JavaScript -->
                </div>
            </section>

            <!-- Popular Artists -->
            <section class="artists-section">
                <div class="section-header">
                    <h2>🎤 Popular Artists</h2>
                    <a href="#">View All</a>
                </div>
                <div class="artists-grid" id="artistsGrid">
                    <!-- Artists will be populated by JavaScript -->
                </div>
            </section>
        </main>
    </div>

    <!-- Music Player -->
    <div class="music-player">
        <div class="player-container">
            <div class="current-song">
                <img src="https://via.placeholder.com/50" alt="Song Cover" id="playerCover">
                <div class="song-info">
                    <span id="playerTitle">Select a song</span>
                    <small id="playerArtist">Artist</small>
                </div>
                <button class="like-btn"><i class="far fa-heart"></i></button>
            </div>
            
            <div class="player-controls">
                <div class="controls-buttons">
                    <button class="control-btn"><i class="fas fa-random"></i></button>
                    <button class="control-btn"><i class="fas fa-step-backward"></i></button>
                    <button class="play-btn" id="playBtn">
                        <i class="fas fa-play"></i>
                    </button>
                    <button class="control-btn"><i class="fas fa-step-forward"></i></button>
                    <button class="control-btn"><i class="fas fa-redo"></i></button>
                </div>
                <div class="progress-container">
                    <span id="currentTime">0:00</span>
                    <div class="progress-bar" id="progressBar">
                        <div class="progress" id="progress"></div>
                    </div>
                    <span id="duration">0:00</span>
                </div>
            </div>
            
            <div class="player-options">
                <button class="control-btn"><i class="fas fa-list"></i></button>
                <button class="control-btn"><i class="fas fa-volume-up"></i></button>
                <div class="volume-slider">
                    <input type="range" min="0" max="100" value="50" id="volumeSlider">
                </div>
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
