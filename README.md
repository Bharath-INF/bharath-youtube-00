# bharath-youtube-00
<!DOCTYPE html>
<html>
    <head>
        <title>YouTube,com clone</title>

        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">


        <link rel="stylesheet" href="styles/header.css">
        <link rel="stylesheet" href="styles/genaral.css">
        <link rel="stylesheet" href="styles/video.css">
        <link rel="stylesheet" href="styles/sidebar.css">

        <style>
            p {
                font-family: Roboto, Arial;
                margin-top: 0;
                margin-bottom: 0;
            }

            body {
                margin: 0;
                padding-top: 80px;
                padding-left: 96px;
                padding-right: 24px;
                background-color: rgb(243, 243, 243);
            }

            .header {
                height: 55px;
                display: flex;
                flex-direction: row;
                justify-content: space-between;
                background-color: white;
                position: fixed;
                top: 0;
                left: 0;
                right: 0;
                z-index: 100;
                border-bottom-width: 1px;
                border-bottom-style: solid;
                border-bottom-color:rgb(224, 220, 220);
            }
        

            .left-section {
                width: 160px;
                display: flex;
                align-items: center;
            }

            .hamburger-menu {
                height: 24px;
                margin-left: 24px;
                margin-right: 24px;
            }

            .youtube-logo {
                height: 20px;
            }

            .middle-section {
                flex: 1;
                margin-left: 60px;
                margin-right: 35px;
                max-width: 500px;
                display: flex;
                align-items: center;
            }

            .search-bar {
            flex: 1;
            height: 36px;
            padding-left: 12px;
            font-size: 16px;
            border-width: 1px;
            border-style: solid;
            border-color: rgb(204, 204, 204);
            border-radius: 2px;
            box-shadow: inset 1px 2px 3px rgba(0, 0, 0, 0.05);
            width: 0;
            }

            .search-bar::placeholder {
                font-family: roboto, arial;
                font-size: 16px;
            }

            .search-button {
                height: 40px;
                width: 66px;
                background-color: rgb(248, 248, 248);
                border-width: 1px;
                border-style: solid;
                border-color:rgb(204, 204, 204);
                margin-left: -1px;
            }

            .search-icon {
                height: 25px;
                margin-top: 4px;
            }

            .voice-search-button {
                height: 40px;
                width: 40px;
                border: none;
                border-radius: 50px;
                margin-left: 12px;
                background-color:rgb(248, 248, 248);
            }

            .voice-icon{
                margin-top: 3px;
                height: 24px;
            }

            .right-section {
                width: 180px;
                margin-right: 20px;
                display: flex;
                align-items: center;
                justify-content: space-between;
                flex-shrink: 0;
            }

            .upload {
                height: 24px;
            }

            .youtube-apps {
                height: 24px;
            }

            .notification {
                height: 24px;
            }

            .notifications-icon-container {
                position:  relative;
            }

            .notifications-count {
                position: absolute;
                top: -2px;
                right: -5px;
                background-color: rgb(204, 0, 0);
                color: white;
                font-family: roboto, arial;
                font-size: 11px;
                padding-left: 5px;
                padding-right: 5px;
                padding-top: 2px;
                padding-bottom: 2px;
                border-radius: 10px;
            }

            .my-channel {
                height: 32px;
                border-radius: 16px;
            }

            .sidebar {
                position: fixed;
                left: 0;
                bottom: 0;
                top: 55px;
                background-color: white;
                width: 72px;
                z-index: 200;
                padding-top: 5px;
            }

            .sidebar-link {
                height: 74px;
                display: flex;
                justify-content: center;
                align-items: center;
                flex-direction: column;
                cursor: pointer;
            }

            .sidebar-link:hover {
                background-color: rgb(232, 231, 231);
            }

            .sidebar-link img {
                height: 24px;
                margin-bottom: 7px;
            }

            .sidebar-link div {
                font-family: roboto, arial;
                font-size: 10px;
            }

            .thumbnail {
                width: 100%;
            }

            .video-title {
                margin-top: 0;
                font-size: 14px;
                font-weight: 500;
                line-height: 20px;
                margin-bottom: 10px;
            }


            .video-info-grid {
                display: grid;
                grid-template-columns: 50px 1fr;
            }

            .profile-1 {
                width: 36px;
                border-radius: 50px;
            }

            .thumbnail-row {
                margin-bottom: 8px;
                position: relative;
            }

            .video-author,
            .video-stats {
                font-size: 12px;
                color: rgb(96, 96, 96);
            }

            .video-author {
                margin-bottom: 4px;
            }

            .video-grid {
                display: grid;
                grid-template-columns: 1fr 1fr 1fr;
                column-gap: 16px;
                row-gap: 40px;
            }

            .video-time {
                font-family: roboto, arial;
                padding-left: 4px;
                padding-right: 4px;
                padding-top: 4px;
                padding-bottom: 4px;
                background-color: black;
                color: white;
                border-radius: 2px;
                position: absolute;
                bottom: 8px;
                right: 5px;
                font-size: 12px;
                font-weight: 500;
            }

        </style>
    </head>
    <body>
        <div class="header">
            <div class="left-section">
                <img class="hamburger-menu" src="bharath.pic/hamburger-menu.svg">
                <img class="youtube-logo" src="bharath.pic/youtube-logo.svg">
            </div>
            <div class="middle-section">
                <input class="search-bar" type="text" placeholder="Search">
                <button class="search-button">
                    <img class="search-icon" src="bharath.pic/search.svg">
                </button>
                <button class="voice-search-button">
                    <img class="voice-icon" src="bharath.pic/voice-search-icon.svg">
                </button>
            </div>
            <div class="right-section">
                <img class="upload" src="bharath.pic/upload.svg">
                <img class="youtube-apps" src="bharath.pic/youtube-apps.svg">
                <div class="notifications-icon-container">
                    <img class="notification" src="bharath.pic/notifications.svg">
                    <div class="notifications-count">3</div>
                </div>
                <img class="my-channel" src="bharath.pic/WhatsApp Image 2024-11-17 at 7.30.27 PM.jpeg">
            </div>
        </div>

        <div class="sidebar">
            <div class="sidebar-link">
                <img src="bharath.pic/home.svg">
                <div>Home</div>
            </div>
            <div class="sidebar-link">
                <img src="bharath.pic/explore.svg">
                <div>Explore</div>
            </div>
            <div class="sidebar-link">
                <img src="bharath.pic/subscriptions.svg">
                <div>Subscriptions</div>
            </div>
            <div class="sidebar-link">
                <img src="bharath.pic/originals.svg">
                <div>Originals</div>
            </div>
            <div class="sidebar-link">
                <img src="bharath.pic/youtube-music.svg">
                <div>YouTube Music</div>
            </div>
            <div class="sidebar-link">
                <img src="bharath.pic/library.svg">
                <div>Library</div>
            </div>
        </div>

        <div class="video-grid">
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720.webp">
                    <div class="video-time">14:20</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/channels4_profile.jpg">
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Gaali Vaaluga Cover Feat. Aditya || Agnyathavasi Latest 2018 || Anirudh Musical || Night Kreators
                        </p>
                        <p class="video-author">
                            Night Kreators
                        </p>

                        <p class="video-stats">
                            4k views &#183; 6 years ago 
                        </p>
                    </div>   
                </div>
            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (1).webp">
                    <div class="video-time">8:22</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/channels4_profile (1).jpg">     
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Bramhi All Time Comedy Scenes | Brahmanandam Ultimate Comedy | Athadu | Adhurs | Aditya Cinemalu
                        </p>
                        <p class="video-author">
                            Aditya Cinemalu
                        </p>
                        <p class="video-stats">
                            301K views &#183; 13 days ago
                        </p>
                    </div>
                </div>


            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (2).webp">
                    <div class="video-time">9:13</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/unnamed.jpg">
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Mufasa: The Lion King | Telugu Trailer | Mahesh Babu | In Cinemas December 20
                        </p>
                        <p class="video-author">
                            Walt Disney Studios India
                        </p>

                        <p class="video-stats">
                           32.8M views &#183; 5 days ago 
                        </p>
                    </div>   
                </div>
            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (3).webp">
                    <div class="video-time">22:09</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/unnamed (1).jpg">     
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Try Not To Laugh Challenge #9
                        </p>
                        <p class="video-author">
                            Markipiler
                        </p>
                        <p class="video-stats">
                            19M views &#183; 4 years ago
                        </p>
                    </div>
                </div>


            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (4).webp">
                    <div class="video-time">11:17</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/channels4_profile (2).jpg">
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            SARIPODHAA SANIVAARAM Trailer - Nani | Priyanka | SJ Suryah | Vivek Athreya | DVV Danayya
                        </p>
                        <p class="video-author">
                            DVV Entertainment
                        </p>

                        <p class="video-stats">
                           20M views &#183; 2 weeks ago 
                        </p>
                    </div>   
                </div>
            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (5).webp">
                    <div class="video-time">19:59</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/channels4_profile (3).jpg">     
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            7 Days Stranded In A Cave
                        </p>
                        <p class="video-author">
                            Mr Beast
                        </p>
                        <p class="video-stats">
                            98M views &#183; 13 days ago
                        </p>
                    </div>
                </div>


            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (6).webp">
                    <div class="video-time">11:10</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/unnamed (2).jpg">     
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Sunil SuperHit Telugu Movie Hilarious Comedy Scene | Best Telugu Movie Comedy Scene | Film Factory
                        </p>
                        <p class="video-author">
                            Film Factory
                        </p>
                        <p class="video-stats">
                            704K views &#183; 3 months ago
                        </p>
                    </div>
                </div>
            </div>
            <div class="video-preview">
                    <div class="thumbnail-row">
                        <img class="thumbnail" src="bharath.pic/hq720 (7).webp">
                        <div class="video-time">11:10</div>
                    </div>
                    <div class="video-info-grid">
                        <div class="channel-picture">
                            <img class="profile-1" src="bharath.pic/unnamed (3).jpg">     
                        </div>
                        <div class="video-info">
                            <p class="video-title">
                                Filmymoji || Middle Class Madhu || 16 Rojula Pandaga || Pelli Killi || Episode 05 || MCM
                            </p>
                            <p class="video-author">
                                Filmymoji
                            </p>
                            <p class="video-stats">
                                1.3M views &#183; 2 days ago
                            </p>
                        </div>
                    </div>
            </div>
            <div class="video-preview">
                <div class="thumbnail-row">
                    <img class="thumbnail" src="bharath.pic/hq720 (8).webp">
                    <div class="video-time">5:00</div>
                </div>
                <div class="video-info-grid">
                    <div class="channel-picture">
                        <img class="profile-1" src="bharath.pic/channels4_profile (4).jpg">     
                    </div>
                    <div class="video-info">
                        <p class="video-title">
                            Master - Chitti Story Video (Telugu) | Thalapathy Vijay | Anirudh Ravichander 
                        </p>
                        <p class="video-author">
                            Sony Music South
                        </p>
                        <p class="video-stats">
                            15M views &#183; 3 years ago
                        </p>
                    </div>
                </div>
        </div>
        </div>

    </body>
</html>
