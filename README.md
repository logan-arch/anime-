# anime-
will have anime and ways to read manga or watch.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manga & Anime Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to the Manga & Anime Website</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#reading">Read Manga</a></li>
            <li><a href="#watching">Watch Anime</a></li>
        </ul>
    </nav>
    <section id="reading">
        <h2>Read Manga</h2>
        <p>
            <a href="https://allmanga.to/">AllManga.to</a>
            <!-- Add more external manga sources here -->
        </p>
    </section>
    <section id="watching">
        <h2>Watch Anime</h2>
        <p>
            <a href="https://www.anime-planet.com/">Anime-Planet</a>
            <!-- Add more external anime sources here -->
        </p>
    </section>
    <footer>
        &copy; 2023 Manga & Anime Website
    </footer>
</body>
</html>
npm install http-proxy
const http = require('http');
const httpProxy = require('http-proxy');

const target = 'http://www.squid-cache.org
//'; // 
const proxy = httpProxy.createProxyServer({});

const server = http.createServer((req, res) => {
  proxy.web(req, res, { target });
});

server.listen(3000); // node your-proxy-server.js
sudo apt-get update
sudo apt-get install squid
http_port 3128
acl localnet src 0.0.0.1-0.255.255.255
acl localnet src 10.0.0.0/8
acl localnet src 100.64.0.0/10
acl localnet src 169.254.0.0/16
acl localnet src 172.16.0.0/12
acl localnet src 192.168.0.0/16
acl localnet src fc00::/7
acl localnet src fe80::/10
acl SSL_ports port 443
acl Safe_ports port 80
acl Safe_ports port 21
acl Safe_ports port 443
acl Safe_ports port 70
acl Safe_ports port 210
acl Safe_ports port 1025-65535
acl Safe_ports port 280
acl Safe_ports port 488
acl Safe_ports port 591
acl Safe_ports port 777
http_access deny !Safe_ports
http_access deny CONNECT !SSL_ports
http_access allow localnet
http_access allow localhost
http_access deny all
http_access allow all
sudo service squid start
