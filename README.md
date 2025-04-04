# daily motivations
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Daily Motivational Quotes to Inspire Your Day">
  <title>Daily Motivation</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      padding: 50px;
      background: #f4f4f4;
    }
    .quote-box {
      background: white;
      padding: 30px;
      border-radius: 10px;
      max-width: 600px;
      margin: 0 auto;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    .quote {
      font-size: 1.5rem;
      font-style: italic;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 1rem;
      border: none;
      background: #333;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background: #555;
    }
  </style>
</head>
<body>
  <h1>Daily Motivation</h1>
  <div class="quote-box">
    <p class="quote" id="quote">Loading...</p>
    <button onclick="generateQuote()">New Quote</button>
  </div>

  <!-- Google AdSense (add your own ad-client ID) -->
  <div style="margin-top: 30px;">
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"
     crossorigin="anonymous"></script>
    <ins class="adsbygoogle"
         style="display:block"
         data-ad-client="ca-pub-XXXXXXXXXXXXXX"
         data-ad-slot="1234567890"
         data-ad-format="auto"
         data-full-width-responsive="true"></ins>
    <script>
         (adsbygoogle = window.adsbygoogle || []).push({});
    </script>
  </div>

  <script>
    const quotes = [
      "Your limitation—it’s only your imagination.",
      "Push yourself, because no one else is going to do it for you.",
      "Great things never come from comfort zones.",
      "Dream it. Wish it. Do it.",
      "Success doesn’t just find you. You have to go out and get it.",
      "The harder you work for something, the greater you’ll feel when you achieve it.",
      "Don’t watch the clock; do what it does. Keep going.",
      "Sometimes later becomes never. Do it now.",
      "Don’t stop when you’re tired. Stop when you’re done.",
      "Wake up with determination. Go to bed with satisfaction."
    ];

    function generateQuote() {
      const randomIndex = Math.floor(Math.random() * quotes.length);
      document.getElementById('quote').innerText = `"${quotes[randomIndex]}"`;
    }

    // Generate one on load
    generateQuote();
  </script>
</body>
</html>
