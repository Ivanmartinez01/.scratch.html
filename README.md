<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Lionel Messi - World Champion</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f3f9ff;
      color: #1c1c1c;
    }
    nav {
      background-color: #0d1b2a;
      color: white;
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 999;
    }
    nav a {
      color: white;
      margin-right: 15px;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .container {
      padding: 30px;
    }
    .section {
      padding: 40px 20px;
      border-bottom: 1px solid #ccc;
    }
    h1, h2 {
      color: black;
    }
    .resume-list ul {
      margin-left: 20px;
    }
    .header {
      background-image: url('Screenshot 2025-04-22 at 11.29.13 PM.png');
      background-size: cover;
      background-position: center;
      color: white;
      padding: 40px;
      text-align: center;
    }
    .worldcup-image {
      width: 100%;
      max-width: 600px;
      margin: 20px 0;
      border-radius: 8px;
    }
    .tableau-embed {
      margin: 30px 0;
    }
    .riddle-box {
      background: #ffffff;
      border-radius: 10px;
      padding: 30px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      max-width: 600px;
      margin: auto;
    }
    button {
      background-color: #0d6efd;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 8px;
      margin-top: 20px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0b5ed7;
    }
    .answer {
      margin-top: 10px;
      color: #2c2c2c;
      font-style: italic;
    }
    .footer {
      background-color: #0d1b2a;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <nav>
    <a href="#resume">Résumé</a>
    <a href="#scratch">World Cup</a>
    <a href="#riddle">Riddle App</a>
  </nav>

  <section class="section" id="resume">
    <div class="container resume-list">
      <h2>Résumé</h2>
      <p><strong>Ivan Martinez</strong> | (801) 367-4722 | martneztino@gmail.com | <a href="https://www.linkedin.com/in/ivanmart1nez" target="_blank">LinkedIn</a></p>
      <p><strong>Education:</strong> Brigham Young University – Marriott School of Business</p>
      <ul>
        <li>Associates in Pre-Business</li>
        <li>Member of the CFFA Business Club</li>
        <li>Proficient in SQL and learning VBA</li>
      </ul>
      <p><strong>Experience:</strong></p>
      <ul>
        <li><strong>ATTYX Home Improvement</strong> – Sales Development Rep (Mar 2024 – Present)<br>
          ▪ Developed persuasive communication through direct sales<br>
          ▪ SDR of the Month 2x, managed client relationships<br>
          ▪ Used data to hit sales targets</li>
        <li><strong>FLO Energy</strong> – D2D Setter (Summer 2023)<br>
          ▪ Rapid rapport building, objection handling, goal-driven</li>
        <li><strong>Vivint Solar</strong> – Inside Sales Rep (Jan 2022 – May 2023)<br>
          ▪ Moved from setting to closing appointments<br>
          ▪ Mastered active listening, communication, objection handling</li>
      </ul>
      <p><strong>Leadership & Service:</strong></p>
      <ul>
        <li><strong>BYU Projects</strong> – Led Excel and VBA-based presentations</li>
        <li><strong>LDS Mission (Raleigh, NC)</strong> – Volunteer Leader (2019–2021)<br>
          ▪ Trained teams of 16, tracked goals, managed Ads</li>
      </ul>
      <p><strong>Awards & Skills:</strong></p>
      <ul>
        <li>Fluent in 2 languages</li>
        <li>Summer sales trip award winner</li>
        <li>High expectations, trial closing, effective communicator</li>
        <li>Studies in finance, marketing, programming</li>
      </ul>
    </div>
  </section>

  <section class="section" id="scratch">
    <div class="header">
      <h1>Soccer & The World Cup</h1>
      <p>The greatest sport on Earth, every four years at its peak.</p>
    </div>
    <div class="container">
      <h2>Why the World Cup is Awesome</h2>
      <ol>
        <li>It brings the world together
          <ul>
            <li>Over 3 billion viewers</li>
            <li>Fan culture from every continent</li>
          </ul>
        </li>
        <li>Stories of Underdogs</li>
        <li>Legends Are Born</li>
      </ol>

      <img src="Screenshot 2025-04-22 at 11.29.13 PM.png" alt="World Cup Trophy" class="worldcup-image">

      <h3 id="video">Watch the 2022 World Cup Glory</h3>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/ZmKy_fnRM_E" title="Lionel Messi - World Champion" frameborder="0" allowfullscreen></iframe>

      <h3>World Cup Viewership Since 2010</h3>
      <div class="tableau-embed">
        <iframe src="https://public.tableau.com/views/WorldCupViewershipData/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link" width="800" height="600"></iframe>
      </div>
    </div>
  </section>

  <section class="section" id="riddle">
    <div class="container">
      <div class="riddle-box">
        <h2>🧠 Riddle Me This</h2>
        <p id="riddle">Click below to get a riddle!</p>
        <p id="answer" class="answer"></p>
        <button onclick="generateRiddle()">New Riddle</button>
      </div>
    </div>
  </section>

  <div class="footer">
    <p>⚽ Built by Ivan Martinez — BYU Web Dev Final Project ⚽</p>
  </div>

  <script>
    const riddles = [
      {
        question: "I speak without a mouth and hear without ears. I have no body, but I come alive with wind. What am I?",
        answer: "An echo."
      },
      {
        question: "What can run but never walks, has a bed but never sleeps, and has a mouth but never eats?",
        answer: "A river."
      },
      {
        question: "I’m tall when I’m young, and I’m short when I’m old. What am I?",
        answer: "A candle."
      },
      {
        question: "I have keys but no locks. I have space but no room. You can enter, but you can’t go outside. What am I?",
        answer: "A keyboard."
      },
      {
        question: "What has to be broken before you can use it?",
        answer: "An egg."
      },
      {
        question: "BONUS: What do you call a riddle that doesn’t make sense?",
        answer: "A ChatGPT original 😅"
      }
    ];

    function generateRiddle() {
      const randIndex = Math.floor(Math.random() * riddles.length);
      document.getElementById('riddle').textContent = riddles[randIndex].question;
      document.getElementById('answer').textContent = "🤫 Click again to reveal the answer...";
      setTimeout(() => {
        document.getElementById('answer').textContent = riddles[randIndex].answer;
      }, 3500);
    }
  </script>
</body>
</html>
