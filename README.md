<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ad Viewer</title>
  <style>
    body, html {
      margin: 0; padding: 0;
      height: 100%; width: 100%;
      display: flex;
      flex-direction: column;
      font-family: Arial, sans-serif;
    }
    header {
      background: #0a84ff;
      color: white;
      text-align: center;
      padding: 15px 0;
      font-size: 18px;
    }
    iframe {
      flex: 1;
      border: none;
      width: 100%;
    }
    footer {
      background: #f0f0f0;
      text-align: center;
      padding: 10px;
      font-size: 14px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      border: none;
      background: #0a84ff;
      color: white;
      border-radius: 5px;
    }
  </style>
</head>
<body>

  <header>Ad Viewer</header>

  <iframe id="adFrame" src="https://data684.click/1dd1637c673a01eefcb0/8121fc0c30/?placementName=default"></iframe>

  <footer>
    <button onclick="reloadAd()">Reload Ad</button>
  </footer>

  <script>
    function reloadAd() {
      const frame = document.getElementById('adFrame');
      frame.src = frame.src; // iframe reload
    }
  </script>

</body>
</html>
