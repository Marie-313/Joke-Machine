<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Computer Joke Machine</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        min-height: 100vh;
        margin: 0;
        background: linear-gradient(
          135deg,
          rgb(255, 168, 168) 10%,
          rgb(252, 255, 0) 100%
        );
      }

      .container {
        background-color: rgb(255, 255, 255);
        padding: 2rem;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(252, 235, 235, 0.1);
        text-align: center;
        max-width: 600px;
        width: 90%;
      }

      button {
        background-color: #c54003;
        color: white;
        padding: 10px 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
        margin-top: 20px;
      }

      button:hover {
        background-color: #030303;
      }

      #joke {
        font-size: 18px;
        margin: 20px 0;
        min-height: 60px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <h1>😄 Computer Joke Machine 😄</h1>
      <div id="joke">Click the button for a joke!</div>
      <button onclick="tellJoke()">Tell me a joke!</button>
    </div>

    <script>
      const jokes = [
        "Why do programmers prefer dark mode? Because light attracts bugs!",
        "Why did the programmer quit his job? Because he didn't get arrays!",
        "What's a computer's favorite snack? Microchips!",
        "Why did the computer go to the doctor? Because it had a virus!",
        "What do you call a computer that sings? A Dell!",
        "Why was the math book sad? Because it had too many problems!",
        "What did the computer do at lunchtime? Had a byte!",
        "Why don't programmers like nature? It has too many bugs!",
        "What did the RAM say to the computer? Let me think about that!",
        "Why did the cookie go to the doctor? Because it was feeling crumbly!",
        "What's a computer's favorite beat? An algorithm!",
        "Why did the computer keep freezing? It left its Windows open!",
        "What do you call a computer floating in the ocean? A Dell-phin!",
        "Why are computers so smart? They listen to their motherboards!",
        "What's a computer's favorite game? Cache catch!",
        "Why did the computer get glasses? Because it couldn't C++!",
        "What do you call a computer superhero? Data Man!",
        "Why did the programmer go broke? Because he used up all his cache!",
        "What's a computer's favorite dance? The digital boogie!",
        "Why don't computers like coffee breaks? They prefer short Java breaks!",
        "What did the computer say to its valentine? You're the Apple of my eye!",
        "Why was the computer cold? It left its Windows open!",
        "What's a computer's favorite dessert? Cookies and cache!",
        "Why did the computer go to therapy? It had too many internal conflicts!",
        "What do you call a computer that tells jokes? A LOL-gorithm!",
        "What did the computer say when it crashed? Byte me!",
        "Why did the programmer always get lost? Because he kept following the recursive path!",
        "What's a computer's favorite type of music? Hard disk rock!",
        "Why did the database administrator leave his wife? She had too many relationships!",
        "What do you call a computer mouse that swears? A cursor!",
      ];

      function tellJoke() {
        const jokeDisplay = document.getElementById("joke");
        const randomIndex = Math.floor(Math.random() * jokes.length);
        jokeDisplay.textContent = jokes[randomIndex];
      }
    </script>
  </body>
</html>
