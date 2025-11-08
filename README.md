<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Live Chat</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #77d5dc;
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 100vh;
    }

    #chat {
      width: 150%;
      max-width: 600px;
      background: white;
      border: 1px solid #ccc;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
      margin-top: 20px;
      padding: 10px;
      overflow-y: auto;
    }

    #messages {
      list-style: none;
      padding: 0;
      flex-grow: 1;
      overflow-y: auto;
    }

    #messages li {
      padding: 8px;
      margin-bottom: 4px;
      border-bottom: 1px solid #eee;
    }

    form {
      display: flex;
      margin-top: 10px;
    }

    input {
      flex: 1;
      padding: 10px;
      border: 1px solid #ccc;
    }

    button {
      padding: 10px;
      background: #007bff;
      color: white;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <h2>💬 Live Chat</h2>
  <div id="chat">
    <ul id="messages"></ul>
    <form id="form">
      <input id="input" autocomplete="off" placeholder="Schreibe eine Nachricht..." />
      <button>Senden</button>
    </form>
  </div>

  <script src="/socket.io/socket.io.js"></script>
  <script src="script.js">albert("hallo world");</script>
</body>
</html>
