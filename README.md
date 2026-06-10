<!DOCTYPE html>
<html lang="da">
<head>
    <meta charset="UTF-8">
    <title>Hvad skal jeg spille?</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
        }

        button {
            padding: 15px 30px;
            font-size: 20px;
            cursor: pointer;
        }

        #resultat {
            margin-top: 30px;
            font-size: 30px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>🎮 Hvad skal jeg spille?</h1>

    <button onclick="vaelgSpil()">
        Vælg et spil
    </button>

    <div id="resultat"></div>

    <script>
        const spil = [
            "League of Legends",
            "Warframe",
            "Dead by Daylight",
            "Elden Ring",
            "Minecraft",
            "Counter-Strike 2"
        ];

        function vaelgSpil() {
            const tilfældigtNummer =
                Math.floor(Math.random() * spil.length);

            document.getElementById("resultat").innerText =
                spil[tilfældigtNummer];
        }
    </script>

</body>
</html>
