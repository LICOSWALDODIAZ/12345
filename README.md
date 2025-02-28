     }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            display: inline-block;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            background: #ff4d4d;
            color: white;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: #cc0000;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2 id="question">¿Cuánto me amas? ❤️</h2>
        <button onclick="nextPhrase()">Muchísimo 💖</button>
        <button onclick="nextPhrase()">Más que todo 💕</button>
        <button onclick="nextPhrase()">Con toda mi alma ❤️</button>
        <br>
        <button onclick="nextQuestion()">Siguiente ➡️</button>
        <h3 id="phrase"></h3>
    </div>

    <script>
        const phrases = [
            "Eres mi razón de ser, mi amor eterno 💖.",
            "Cada latido de mi corazón dice tu nombre 💓.",
            "Eres el mejor regalo que la vida me ha dado 🎁💕.",
            "No hay día en que no agradezca por tenerte a mi lado 🌹.",
            "Te amo más de lo que las palabras pueden expresar 💘."
        ];
        let index = 0;

        function nextPhrase() {
            document.getElementById("phrase").innerText = phrases[index];
            index = (index + 1) % phrases.length;
        }
    </script>
</body>
</html>
