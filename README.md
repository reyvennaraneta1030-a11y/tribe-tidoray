<!DOCTYPE html>
<html lang="en">
<head>
    
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
            margin-bottom: 5px;
        }

        header p {
            font-size: 20px;
        }

        /* ================= MENU ================= */

        .menu {
            height: 78vh;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            flex-wrap: wrap;
            padding: 20px;
        }

        .menu a {
            text-decoration: none;
            color: white;
            background: #8b5e3c;
            padding: 25px 35px;
            border-radius: 20px;
            font-size: 25px;
            font-weight: bold;
            transition: 0.3s;
        }

        .menu a:hover {
            background: #5b3a29;
            transform: scale(1.05);
        }

        /* ================= POPUP ================= */

        .popup {
            display: none;
            position: fixed;
            inset: 0;
            background: rgba(0, 0, 0, 0.65);
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .popup:target {
            display: flex;
        }

        .popup-box {
            background: #fffaf2;
            width: 90%;
            max-width: 600px;
            max-height: 80vh;
            overflow-y: auto;
            padding: 30px;
            border-radius: 20px;
            text-align: left;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        .popup-box h2 {
            color: #5b3a29;
            margin-bottom: 15px;
            text-align: center;
        }

        .popup-box p {
            line-height: 1.7;
            margin-bottom: 15px;
        }

        .close {
            display: block;
            text-align: center;
            text-decoration: none;
            background: #8b5e3c;
            color: white;
            padding: 12px;
            border-radius: 10px;
            margin-top: 20px;
        }

        .close:hover {
            background: #5b3a29;
        }

        
    </style>
</head>

<body>

    <!-- ================= HEADER ================= -->

    <header>
        <h1>Tiduray Culture</h1>
        <p style="font-size:180%">Discover the culture, traditions, beliefs, and fun facts of the Tiduray people.</p>
    </header>

 <!-- ================= HOME ================= -->

    <section id="home">

        <div class="home-content">
            <center>
            <h1>Welcome!</h1>

            <p style="font-size:240%;">
                The Tiduray, also known as Teduray or Tiruray,<br> are one of the Indigenous peoples of Mindanao in the Philippines.<br> Their communities are traditionally<br> associated with areas of Maguindanao and nearby parts of Central Mindanao.

The Tiduray<br> have a rich cultural heritage expressed through their language, <br> traditional knowledge, clothing, crafts, music, stories, and relationship with nature.
            </p>

           </center>

    <!-- ================= MENU ================= -->

    <div class="menu">

        <a href="#culture">Culture</a>
        <a href="#traditions">Traditions</a>
        <a href="#beliefs">Beliefs</a>
        <a href="#facts">Fun Facts</a>

    </div>

    <!-- ================= CULTURE POPUP ================= -->

    <div id="culture" class="popup">

        <div class="popup-box">

            <h2>Tiduray Culture</h2>

            <p>
                The Tiduray, also known as Teduray, are an Indigenous
                people of Mindanao, particularly in parts of Maguindanao
                del Sur and nearby areas.
            </p>

            <p>
                Their culture includes traditional clothing, music,
                weaving, farming, and strong community relationships.
            </p>

            <p>
                They are known for preserving their identity through
                language, customs, and traditional practices.
            </p>

            <a href="#" class="close">Close</a>

        </div>

    </div>

    <!-- ================= TRADITIONS POPUP ================= -->

    <div id="traditions" class="popup">

        <div class="popup-box">

            <h2>Tiduray Traditions</h2>

            <p>
                Traditional Tiduray communities value cooperation,
                respect for elders, and the passing of knowledge
                from one generation to another.
            </p>

            <p>
                Traditional weaving, music, dances, and community
                gatherings are important parts of their cultural
                expression.
            </p>

            <p>
                Many traditions are connected to their relationship
                with nature and their way of life.
            </p>

            <a href="#" class="close">Close</a>

        </div>

    </div>

    <!-- ================= BELIEFS POPUP ================= -->

    <div id="beliefs" class="popup">

        <div class="popup-box">

            <h2>Tiduray Beliefs</h2>

            <p>
                Tiduray traditional beliefs include respect for
                nature, ancestors, and the spiritual world.
            </p>

            <p>
                Their traditional knowledge and practices reflect
                the importance of harmony between people and their
                environment.
            </p>

            <p>
                Beliefs and customs may vary among communities and
                families.
            </p>

            <a href="#" class="close">Close</a>

        </div>

    </div>

    <!-- ================= FUN FACTS POPUP ================= -->

    <div id="facts" class="popup">

        <div class="popup-box">

            <h2>Fun Facts About the Tiduray</h2>

            <p>
                • The Tiduray are also called Teduray.
            </p>

            <p>
                • They are an Indigenous people of Mindanao.
            </p>

            <p>
                • Traditional weaving is an important part of
                their cultural heritage.
            </p>

            <p>
                • Their culture includes traditional music,
                dances, and community practices.
            </p>

            <p>
                • They have their own language and cultural identity.
            </p>

            <a href="#" class="close">Close</a>

        </div>

    </div>

</body>
</html>
