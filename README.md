<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Calculatrice Yu Gi Oh</title>
</head>
<body>
    <div class="calculator">
        <div class="players">
          <div class="player">
            <label for="player1Name">Player 1</label>
            <input type="text" id="player1Name" placeholder="Enter Name">
            <label for="player1"></label>
            <input type="text" id="player1" value="8000" readonly>
            <input type="number" id="adjustment1" placeholder="Adjustment">
            <button onclick="adjustLifePoints(1, 1)">+</button>
            <button onclick="adjustLifePoints(1, -1)">-</button>
            <button onclick="divideByTwo(1)">/2</button>
          </div>
          <div class="player">
            <label for="player2Name">Player 2</label>
            <input type="text" id="player2Name" placeholder="Enter Name">
            <label for="player2"></label>
            <input type="text" id="player2" value="8000" readonly>
            <input type="number" id="adjustment2" placeholder="Adjustment">
            <button onclick="adjustLifePoints(2, 1)">+</button>
            <button onclick="adjustLifePoints(2, -1)">-</button>
            <button onclick="divideByTwo(2)">/2</button>
          </div>
        </div>
        <div class="result" id="result"></div>
        <button onclick="restartGame()">Restart Game</button>
      </div>
      <div class="history" id="history"></div>
    <script src="script.js"></script>
  </body>
</html>
