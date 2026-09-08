<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>오늘 저녁 뭐 먹지?</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, system-ui, Roboto, sans-serif;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 99%, #fecfef 100%);
        }

        .container {
            background-color: white;
            padding: 3rem 2rem;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 400px;
            width: 90%;
        }

        h1 {
            color: #333;
            font-size: 1.8rem;
            margin-bottom: 2rem;
        }

        .result-box {
            min-height: 180px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            margin-bottom: 2rem;
            background-color: #f8f9fa;
            border-radius: 15px;
            padding: 1rem;
        }

        .emoji {
            font-size: 5rem;
            margin-bottom: 0.5rem;
            transition: transform 0.2s ease;
        }

        .menu-name {
            font-size: 1.5rem;
            font-weight: bold;
            color: #ff6b6b;
        }

        button {
            background-color: #ff6b6b;
            color: white;
            border: none;
            padding: 1rem 2rem;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
            transition: all 0.2s ease;
            width: 100%;
        }

        button:hover {
            background-color: #ff5252;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255, 107, 107, 0.6);
        }

        button:active {
            transform: translateY(0);
        }

        /* 쿵쾅 애니메이션 효과 */
        .bounce {
            animation: bounce 0.4s ease;
        }

        @keyframes bounce {
            0% { transform: scale(0.3); opacity: 0; }
            50% { transform: scale(1.1); }
            70% { transform: scale(0.9); }
            100% { transform: scale(1); opacity: 1; }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>🍽️ 오늘 뭐 먹지?</h1>
        
        <div class="result-box">
            <div id="emoji" class="emoji">❓</div>
            <div id="menu-name" class="menu-name">버튼을 눌러보세요!</div>
        </div>

        <button onclick="recommendMenu()">오늘 먹을 저녁 추천</button>
    </div>

    <script>
        // 저녁 메뉴 데이터베이스 (이모지 & 메뉴명)
        const menuList = [
            { emoji: "🍕", name: "피자" },
            { emoji: "🍔", name: "햄버거" },
            { emoji: "🍗", name: "치킨" },
            { emoji: "🍜", name: "라면/우동" },
            { emoji: "🍣", name: "초밥" },
            { emoji: "🍱", name: "돈까스/도시락" },
            { emoji: "🥩", name: "삼겹살/소고기" },
            { emoji: "🍛", name: "카레" },
            { emoji: "🥘", name: "부대찌개/전골" },
            { emoji: "🍲", name: "김치찌개/된장찌개" },
            { emoji: "🌮", name: "타코/멕시칸" },
            { emoji: "🍝", name: "파스타" },
            { emoji: "🥟", name: "만두/중화요리" },
            { emoji: "🥗", name: "샐러드/포케" },
            { emoji: "🍢", name: "떡볶이/분식" },
            { emoji: "🥣", name: "국밥" },
            { emoji: "🥙", name: "케밥/샌드위치" }
        ];

        function recommendMenu() {
            const emojiElement = document.getElementById("emoji");
            const nameElement = document.getElementById("menu-name");

            // 애니메이션 초기화
            emojiElement.classList.remove("bounce");

            // 랜덤 메뉴 선택
            const randomIndex = Math.floor(Math.random() * menuList.length);
            const selectedMenu = menuList[randomIndex];

            // 잠깐의 시각적 효과 후 화면 변경
            setTimeout(() => {
                emojiElement.textContent = selectedMenu.emoji;
                nameElement.textContent = selectedMenu.name;
                
                // 애니메이션 다시 적용
                emojiElement.classList.add("bounce");
            }, 50);
        }
    </script>
</body>
</html>