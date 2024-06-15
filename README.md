<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SpotyGen</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #000000;
            color: #fff;
            text-align: center;
            padding: 50px;
        }
        .container {
            background-color: #191414;
            border-radius: 10px;
            padding: 20px;
            display: inline-block;
        }
        h1 {
            color: #ffffff;
        }
        .account {
            background-color: #fff;
            color: #000;
            border-radius: 5px;
            padding: 10px;
            margin: 10px 0;
        }
        button {
            background-color: #7a7979;
            border: none;
            color: #fff;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #14833b;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Spotify</h1> 
        <button onclick="generateAccount()">Générer un compte</button> </p> 
        <div id="accounts"></div>




    </div>

    <script>
        function generateAccount() {
            const accounts = [
                {email: "anikaki@gmail.com", password: "HZneZwC54r"},
                {email: "adriennedubois@gmail.com", password: "iFu7APVkc"},            
                {email: "leheumeerte@gmail.com", password: "pduVM4JmV"},
                {email: "sposponutea.derter@gmail.com", password: "pwq2PkDMNchord"},
                {email: "fullnewsdelaterre@gmail.com", password: "f14KwXKpwP"},
                {email: "lauragiatar@gmail.com", password: "NuGUabgB36"}
            ];
            const randomAccount = accounts[Math.floor(Math.random() * accounts.length)];
            const accountDiv = document.createElement("div");
            accountDiv.className = "account";
            accountDiv.innerHTML = `<p>Email: ${randomAccount.email}</p><p>Mot de passe: ${randomAccount.password}</p>`;
            document.getElementById("accounts").appendChild(accountDiv);
        }
    </script>
</body>
</p>

<div class="container">
    <h1>Disney Plus</h1>    
    <button onclick="generateaccount()">Générer un compte</button>
    <div id="accounts"></div>
</div>
<p>! Le Gen de compte Disney Plus est en cours de developpement ! </p>




</html>
