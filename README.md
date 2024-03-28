# 3_in_1-game-webpage

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3-in-1 Game Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: hsl(243, 66%, 45%);
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        nav {
            background-color: #444;
            color: #fff;
            padding: 10px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin-right: 10px;
        }
        .game-link {
            display: inline-block;
            padding: 10px;
            border-radius: 5px;
            text-decoration: none;
            color: #fff;
            transition: background-color 0.3s;
        }

        #game1-link {
            background-color: #FF5733; 
        }

        #game2-link {
            background-color: #5DADE2; 
        }

        #game3-link {
            background-color: #58D68D; 
        }

        .game-link:hover {
            background-color: #666; 
        }
        main {
            padding: 20px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        section {
            margin-bottom: 20px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            background-color: #fff;
            width: calc(33.40% - 20px);
            margin-right: 20px;
            display: flex;
            flex-direction: column;
        }
        section:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }
        section h2 {
            background-color: #333;
            color: #fff;
            margin: 0;
            padding: 10px;
            text-align: center;
        }
        .game-box {
            flex-grow: 3;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 10px 10px 0 0;
        }
        .game-info {
            padding: 20px;
            text-align: center;
        }
        .game-info p {
            margin: 0;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <header>
        <h1>3-in-1 Game</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#game1" id="game1-link" class="game-link">Game 1</a></li>
            <li><a href="#game2" id="game2-link" class="game-link">Game 2</a></li>
            <li><a href="#game3" id="game3-link" class="game-link">Game 3</a></li>
        </ul>
    </nav>
    <main>
        <section id="game1">
            <h2>Game 1</h2>
            <div class="game-box">
                <img src="egg-catcher.png" alt="Game 1 Image">
                <div class="game-info" id="game1_output"></div>
            </div>
        </section>
        <section id="game2">
            <h2>Game 2</h2>
            <div class="game-box">
                <img src="image.png" alt="Game 2 Image">
                <div class="game-info" id="game2_output"></div>
            </div>
        </section>
        <section id="game3">
            <h2>Game 3</h2>
            <div class="game-box">
                <img src="match-making.png" alt="Game 3 Image">
                <div class="game-info" id="game3_output"></div>
            </div>
        </section>
    </main>
</body>
</html>
