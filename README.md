# sorry-sayang1

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Untuk Isteri Tersayang</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #ffe6e6;
            color: #333;
            text-align: center;
            padding: 20px;
        }
        h1 {
            color: #ff4d4d;
        }
        button {
            background-color: #ff4d4d;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            margin: 10px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #e63939;
        }
        #response {
            margin-top: 20px;
            font-size: 18px;
            color: #004d00;
        }
        #dynamicButton {
            position: relative;
        }
    </style>
</head>
<body>
    <h1>For my wifeyyy, my everything.. Nuur Ain Imanina</h1>
    <p>Sayang, sayang tahu kan baby cintakan and obses dengan sayang sorang je dan akan kekal sayang sorang sampai bila ii and baby tak mampu hidup takde sayang? Sayang tahu kan</p>
    <p>Tapi, baby tahu sayang baby pun buat salah, buat silap, bagi sayang terasa hati, sakit hati, kecewa, serabut, tak suka, macam ii lagi lah.. baby minta maaf sangat sayang.. sayang maafkan baby tak</p>
    <button onclick="reply('Ya, sayang maafkan baby')">Ya, sayang maafkan baby ❤️</button>
    <button id="dynamicButton" onclick="moveAndChange()">Boleh tapi ada syarat 🤔</button>
    <div id="response"></div>

    <script>
        function reply(message) {
            const responseDiv = document.getElementById('response');
            if (message === 'Ya, sayang maafkan baby') {
                responseDiv.innerHTML = "Terima kasih, sayang! baby janji untuk jadi lebih baik 💖";
            }
        }

        function moveAndChange() {
            const button = document.getElementById('dynamicButton');
            const responseDiv = document.getElementById('response');
            
            // Randomize button position
            const randomX = Math.floor(Math.random() * window.innerWidth * 0.8);
            const randomY = Math.floor(Math.random() * window.innerHeight * 0.8);
            button.style.position = "absolute";
            button.style.left = `${randomX}px`;
            button.style.top = `${randomY}px`;
            
            // Change button text randomly
            const texts = [
                "sayang maafkan kalau baby ikut syarat sayang ni 🤔",
                "kalau baby nak sayang maafkan, baby kena buat something",
                "tak tahu baby",
                "sayang nak baby ubah sesuatu",
                "nak sayang maafkan tak? ikut cakap sayang, takleh bantah"
            ];
            button.innerHTML = texts[Math.floor(Math.random() * texts.length)];
            
            // Encourage interaction
            responseDiv.innerHTML = "sayang maafkan baby terus yaa😉";
        }
    </script>
</body>
</html>
