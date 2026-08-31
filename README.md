
<html lang="en">
<head>
    
    <div name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Tiduray Culture</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f4eee3;
            color: #333;
            height: 100vh;
            overflow: hidden;
        }

        /* ================= HEADER ================= */

        header {
            height: 22vh;
            background: linear-gradient(135deg, #5b3a29, #9b6b43);
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        header h1 {
            font-size: 45px;
            margin-bottom: 8px;
        }

        header p {
            font-size: 18px;
        }

        /* ================= NAVIGATION ================= */

        nav {
            height: 10vh;
            background: #3e2723;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
        }

        nav button {
            background: transparent;
            color: white;
            border: 2px solid #c49a6c;
            padding: 10px 18px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 15px;
            font-weight: bold;
        }

        nav button:hover {
            background: #c49a6c;
            color: #3e2723;
        }

        /* ================= HOME ================= */

        #home {
            height: 58vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .home-content {
            width: 80%;
            max-width: 750px;
        }

        .home-content h2 {
            color: #654321;
            font-size: 35px;
            margin-bottom: 15px;
        }

        .home-content p {
            font-size: 18px;
            line-height: 1.7;
        }

        /* ================= POPUP ================= */

        .popup {
            display: none;

            position: fixed;
            z-index: 10;

            top: 50%;
            left: 50%;

            transform: translate(-50%, -50%);

            width: 80%;
            max-width: 850px;
            height: 70vh;

            background: white;

            border-radius: 15px;

            box-shadow: 0 10px 40px rgba(0,0,0,0.4);

            padding: 35px;

            overflow-y: auto;
        }

        .popup.active {
            display: block;
        }

        .popup h2 {
            color: #654321;
            font-size: 32px;
            margin-bottom: 20px;
            text-align: center;
        }

        .popup h3 {
            color: #805a3b;
            margin-top: 18px;
            margin-bottom: 7px;
        }

        .popup p {
            line-height: 1.6;
            margin-bottom: 12px;
        }

        .popup ul {
            margin-left: 25px;
            line-height: 1.7;
        }

        /* ================= CLOSE BUTTON ================= */

        .close {
            position: absolute;

            top: 12px;
            right: 18px;

            border: none;
            background: #805a3b;
            color: white;

            width: 35px;
            height: 35px;

            border-radius: 50%;

            font-size: 20px;
            cursor: pointer;
        }

        .close:hover {
            background: #5b3a29;
        }

        /* ================= CARDS ================= */

        .cards {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin-top: 15px;
        }

        .card {
            background: #f8eee2;
            padding: 18px;
            border-radius: 10px;
            border-left: 5px solid #9b6b43;
        }

        .card h3 {
            margin-top: 0;
        }

        /* ================= FOOTER ================= */

        footer {
            height: 10vh;
            background: #3e2723;
            color: white;

            display: flex;
            justify-content: center;
            align-items: center;

            text-align: center;
        }

        /* ================= MOBILE ================= */

        @media (max-width: 650px) {

            header h1 {
                font-size: 30px;
            }

            header p {
                font-size: 14px;
            }

            nav {
                gap: 5px;
            }

            nav button {
                padding: 8px 10px;
                font-size: 12px;
            }

            .popup {
                width: 90%;
                height: 75vh;
                padding: 25px;
            }

            .cards {
                grid-template-columns: 1fr;
            }
        }
    </style>

<body>

    <!-- ================= HEADER ================= -->

    <header>
        <h1>The Tiduray People</h1>

        <p>
            Discover Their Culture, Traditions, Beliefs and Heritage
        </p>
    </header>


    <!-- ================= NAVIGATION ================= -->

    <nav>

        <button onclick="openPopup('culture')">
            Culture
        </button>

        <button onclick="openPopup('traditions')">
            Traditions
        </button>

        <button onclick="openPopup('beliefs')">
            Beliefs
        </button>

        <button onclick="openPopup('facts')">
            Fun Facts
        </button>

    </nav>


    <!-- ================= HOME ================= -->

    <section id="home">

        <div class="home-content">

            <h1>Welcome!</h1>

            <p style="font-size:150%;">
                The Tiduray, also known as Teduray or Tiruray, are one of the Indigenous peoples of Mindanao in the Philippines. Their communities are traditionally associated with areas of Maguindanao and nearby parts of Central Mindanao.

The Tiduray have a rich cultural heritage expressed through their language, traditional knowledge, clothing, crafts, music, stories, and relationship with nature.
            </p>

           

        </div>

    </section>


    <!-- ================================================= -->
    <!-- ================= CULTURE POPUP ================= -->
    <!-- ================================================= -->

    <div id="culture" class="popup">

        <button class="close" onclick="closePopup('culture')">
            ×
        </button>

        <h2> Tiduray Culture</h2>

        <p>
            Tiduray culture includes traditional knowledge,
            crafts, music, stories, family relationships, and
            a strong connection with the natural environment.
        </p>

        <div class="cards">

            <div class="card">
                <h3>Traditional Crafts</h3>

                <p>
                    Weaving, beadwork, basketry, and other
                    handicrafts are important expressions of
                    cultural identity.
                </p>
            </div>

            <div class="card">
                <h3>Music</h3>

                <p>
                    Traditional songs and musical instruments
                    can be part of cultural and community activities.
                </p>
            </div>

            <div class="card">
                <h3>Oral Tradition</h3>

                <p>
                    Stories, legends, songs, and knowledge
                    can be passed from elders to younger generations.
                </p>
            </div>

            <div class="card">
                <h3>Nature</h3>

                <p>
                    Traditional knowledge includes forests,
                    plants, animals, farming, rivers, and
                    the surrounding environment.
                </p>
            </div>

        </div>

    </div>


    <!-- ================================================= -->
    <!-- ================ TRADITIONS POPUP =============== -->
    <!-- ================================================= -->

    <div id="traditions" class="popup">

        <button class="close" onclick="closePopup('traditions')">
            ×
        </button>

        <h2>🪶 Tiduray Traditions</h2>

        <h3>Traditional Clothing</h3>

        <p>
            Traditional clothing may include handwoven
            textiles, decorative patterns, beadwork,
            and accessories. Styles can differ between communities.
        </p>


        <h3>Weaving</h3>

        <p>
            Weaving is an important traditional skill.
            It can help preserve cultural knowledge and
            demonstrate the creativity and skills of artisans.
        </p>


        <h3>Community Cooperation</h3>

        <p>
            Cooperation between family and community members
            is an important part of traditional life.
        </p>


        <h3>Storytelling</h3>

        <p>
            Elders can play an important role in passing
            stories, history, values, and knowledge to
            younger generations.
        </p>


        <h3>Important Traditional Values</h3>

        <ul>
            <li>Respect for elders</li>
            <li>Community cooperation</li>
            <li>Preservation of traditional skills</li>
            <li>Respect for nature</li>
            <li>Passing knowledge to younger generations</li>
        </ul>

    </div>


    <!-- ================================================= -->
    <!-- ================= BELIEFS POPUP ================= -->
    <!-- ================================================= -->

    <div id="beliefs" class="popup">

        <button class="close" onclick="closePopup('beliefs')">
            ×
        </button>

        <h2> Tiduray Beliefs</h2>

        <p>
            Traditional Tiduray beliefs have included a
            strong relationship between people, nature,
            and the spiritual world.
        </p>


        <h3>Respect for Nature</h3>

        <p>
            Nature has an important place in traditional
            Tiduray life and worldview. Forests, rivers,
            plants, and animals are part of their environment
            and traditional knowledge.
        </p>


        <h3>Spiritual World</h3>

        <p>
            Traditional Tiduray worldview has included
            beliefs concerning spirits and supernatural beings.
            Rituals and customary practices have historically
            been connected with important events and the environment.
        </p>


        <h3>Respect for Elders</h3>

        <p>
            Elders are important sources of traditional
            knowledge, stories, history, and cultural practices.
        </p>


        <h3>Remember</h3>

        <p>
            Not every Tiduray person follows exactly the same
            beliefs today. Culture and beliefs can differ between
            communities and families and can change over time.
        </p>

    </div>


    <!-- ================================================= -->
    <!-- ================= FACTS POPUP =================== -->
    <!-- ================================================= -->

    <div id="facts" class="popup">

        <button class="close" onclick="closePopup('facts')">
            ×
        </button>

        <h2> Fun Facts About the Tiduray</h2>

        <div class="cards">

            <div class="card">
                <h3>1. Indigenous People</h3>

                <p>
                    The Tiduray are an Indigenous people
                    traditionally associated with areas of
                    Central Mindanao.
                </p>
            </div>


            <div class="card">
                <h3>2. Their Own Language</h3>

                <p>
                    The Tiduray language belongs to the
                    Austronesian language family.
                </p>
            </div>


            <div class="card">
                <h3>3. Weaving</h3>

                <p>
                    Traditional weaving and handicrafts
                    are important parts of their cultural heritage.
                </p>
            </div>


            <div class="card">
                <h3>4. Connection With Nature</h3>

                <p>
                    Traditional knowledge includes plants,
                    forests, farming, animals, and the environment.
                </p>
            </div>


            <div class="card">
                <h3>5. Oral Tradition</h3>

                <p>
                    Stories and traditional knowledge can
                    be passed from elders to younger generations.
                </p>
            </div>


            <div class="card">
                <h3>6. Different Names</h3>

                <p>
                    Tiduray, Teduray, and Tiruray are spellings
                    used in different sources for the same
                    Indigenous cultural group.
                </p>
            </div>

        </div>

    </div>


    <!-- ================= FOOTER ================= -->

    <footer>

        <p>
            © 2026 Tiduray Culture Website | Educational Project
        </p>

    </footer>


    <!-- ================= JAVASCRIPT ================= -->

    <script>

        function openPopup(id) {

            document.getElementById(id).classList.add("active");

        }


        function closePopup(id) {

            document.getElementById(id).classList.remove("active");

        }


        // Close popup when pressing ESC

        document.addEventListener("keydown", function(event) {

            if (event.key === "Escape") {

                document.querySelectorAll(".popup").forEach(function(popup) {

                    popup.classList.remove("active");

                });

            }

        });

    </script>

</body>
</html>
