# RellimMC

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RellimMC | Minecraft Server</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #101b16;
    color: white;
}

header {
    background: #17291e;
    padding: 22px 8%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 27px;
    font-weight: bold;
    color: #55ef83;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 18px;
}

.hero {
    text-align: center;
    padding: 110px 20px;
    background:
    linear-gradient(#0009, #000b),
    url("https://images.unsplash.com/photo-1607513746994-51f730a44832?w=1600");
    background-size: cover;
    background-position: center;
}

.hero h1 {
    font-size: clamp(42px, 8vw, 75px);
    color: #55ef83;
    text-shadow: 0 4px 15px black;
}

.hero p {
    font-size: 19px;
    margin: 20px;
}

button {
    padding: 15px 25px;
    border: none;
    border-radius: 8px;
    background: #36d66a;
    color: #102017;
    font-weight: bold;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background: #72ff99;
}

.container {
    width: 85%;
    max-width: 1000px;
    margin: 55px auto;
    text-align: center;
}

h2 {
    color: #55ef83;
    margin-bottom: 25px;
    font-size: 32px;
}

.server-box {
    background: #1d3025;
    padding: 30px;
    border-radius: 15px;
    margin: 25px auto;
}

.ip {
    color: #55ef83;
    font-size: 22px;
    margin: 20px;
    font-weight: bold;
    overflow-wrap: anywhere;
}

.cards {
    display: grid;
    grid-template-columns:
    repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
}

.card {
    background: #1d3025;
    padding: 30px;
    border-radius: 12px;
}

.card h3 {
    color: #55ef83;
    margin-bottom: 15px;
}

.card p {
    line-height: 1.6;
}

footer {
    text-align: center;
    background: #17291e;
    padding: 30px;
    color: #aaa;
}

</style>
</head>

<body>

<header>
    <div class="logo">⛏ RellimMC</div>

    <nav>
        <a href="#home">Home</a>
        <a href="#server">Server</a>
        <a href="#rules">Rules</a>
    </nav>
</header>

<section class="hero" id="home">
    <h1>WELCOME TO RELLIMMC</h1>

    <p>Your next Minecraft adventure starts here!</p>

    <button onclick="copyIP()">
        COPY SERVER IP
    </button>
</section>

<section class="container" id="server">
    <h2>🌍 JOIN OUR SERVER</h2>

    <div class="server-box">
        <p>Java Server Address</p>

        <div class="ip" id="serverIP">
            RellimMC.aternos.me
        </div>

        <button onclick="copyIP()">
            📋 COPY IP
        </button>
    </div>
</section>

<section class="container">
    <h2>⚔️ WHY JOIN RELLIMMC?</h2>

    <div class="cards">

        <div class="card">
            <h3>🌍 Adventure</h3>
            <p>Explore the world and discover new places.</p>
        </div>

        <div class="card">
            <h3>👥 Community</h3>
            <p>Meet friends and play Minecraft together.</p>
        </div>

        <div class="card">
            <h3>⛏️ Survival</h3>
            <p>Gather resources, build and survive.</p>
        </div>

    </div>
</section>

<section class="container" id="rules">
    <h2>📜 SERVER RULES</h2>

    <div class="server-box">
        <p>1. Respect other players.</p>
        <br>
        <p>2. No cheating or hacking.</p>
        <br>
        <p>3. No griefing.</p>
        <br>
        <p>4. Have fun!</p>
    </div>
</section>

<footer>
    <p>© 2026 RellimMC | Minecraft Community</p>
    <p>Not affiliated with Mojang or Microsoft.</p>
</footer>

<script>
function copyIP() {
    navigator.clipboard.writeText(
        "RellimMC.aternos.me"
    ).then(() => {
        alert("Server IP copied! Join RellimMC!");
    }).catch(() => {
        alert("Server IP: RellimMC.aternos.me");
    });
}
</script>

</body>
</html>
