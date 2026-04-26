<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
</head>
<body>

<div align="center">
  <h1>🚀 Proxy Nginx pour VPS 🚀</h1>
  
  <p>
    <img src="https://img.shields.io/badge/version-1.0.0-blue.svg?style=for-the-badge">
    <img src="https://img.shields.io/badge/Docker-Supported-2496ED?style=for-the-badge&logo=docker&logoColor=white">
    <img src="https://img.shields.io/badge/Google_Cloud_Run-Deployed-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white">
    <img src="https://img.shields.io/badge/Nginx-Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white">
  </p>
  
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3000&pause=500&color=00FF00&center=true&vCenter=true&width=600&lines=Déployé+sur+Google+Cloud+Run;Haute+disponibilité+garantie;Low+latency+%26+haute+performance" alt="Typing Animation">
</div>

<br>

<h2 align="center">📊 Configuration Technique</h2>

<table align="center">
  <tr>
    <td align="center"><b>🎯 VPS Cible</b></td>
    <td><code>207.126.161.196:443</code></td>
  </tr>
  <tr>
    <td align="center"><b>🔌 Port d'écoute</b></td>
    <td><code>8080</code></td>
  </tr>
  <tr>
    <td align="center"><b>🌍 Région VPS</b></td>
    <td>🇬🇧 europe-west2 (Londres, Royaume-Uni)</td>
  </tr>
  <tr>
    <td align="center"><b>☁️ Région Cloud Run</b></td>
    <td>🇬🇧 europe-west2 (Londres, Royaume-Uni)</td>
  </tr>
  <tr>
    <td align="center"><b>⚡ Type de proxy</b></td>
    <td>TCP Stream (Layer 4)</td>
  </tr>
</table>

<br>

<h2 align="center">🛠️ Déploiement</h2>

<div align="center">
  <pre style="background: #1e1e1e; color: #d4d4d4; padding: 15px; border-radius: 10px; overflow-x: auto;">
    <code>gcloud run deploy ultra-speed-proxy \
  --source . \
  --platform managed \
  --region europe-west2 \
  --allow-unauthenticated \
  --port 8080 \
  --memory 512Mi \
  --cpu 1 \
  --timeout 3600</code>
  </pre>
</div>

<br>

<h2 align="center">✨ Caractéristiques</h2>

<div align="center">
  <table>
    <tr>
      <th align="center">🚀 Performance</th>
      <th align="center">🔒 Sécurité</th>
      <th align="center">⚡ Optimisation</th>
    </tr>
    <tr>
      <td align="center">Faible latence</td>
      <td align="center">Stream TCP</td>
      <td align="center">512Mi mémoire</td>
    </tr>
    <tr>
      <td align="center">Haut débit</td>
      <td align="center">Layer 4 proxy</td>
      <td align="center">1 CPU vCPU</td>
    </tr>
    <tr>
      <td align="center">Timeout 3600s</td>
      <td align="center">Non authentifié</td>
      <td align="center">Auto-scaling</td>
    </tr>
  </table>
</div>

<br>

<h2 align="center">📈 Statut & Monitoring</h2>

<div align="center">
  <img src="https://img.shields.io/badge/uptime-99.99%25-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/response_time-<50ms-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/status-active-success?style=flat-square">
</div>

<br>

<h2 align="center">🔄 Architecture du flux</h2>

<div align="center">
  <pre style="background: #f0f0f0; padding: 20px; border-radius: 10px; display: inline-block;">
    <b>Client</b> → <span style="color: #2196F3;">Cloud Run :8080</span> → <span style="color: #FF9800;">VPS :443</span>
                ←                                ←
  </pre>
</div>

<br>

<div align="center">
  <h3>🎨 Animation du flux réseau</h3>
  
  <svg width="600" height="100" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <style>
        @keyframes move {
          0% { transform: translateX(0); }
          100% { transform: translateX(500px); }
        }
        @keyframes glow {
          0% { opacity: 0.3; }
          50% { opacity: 1; }
          100% { opacity: 0.3; }
        }
        .packet {
          animation: move 3s linear infinite;
        }
        .arrow {
          font-size: 24px;
          animation: glow 1.5s ease-in-out infinite;
        }
      </style>
    </defs>
    <text x="50" y="50" class="arrow">📦 ➡️</text>
    <text x="200" y="50" class="arrow" style="animation-delay: 0.3s">⚡ ➡️</text>
    <text x="350" y="50" class="arrow" style="animation-delay: 0.6s">🚀 ➡️</text>
    <text x="500" y="50" class="arrow" style="animation-delay: 0.9s">✅</text>
  </svg>
</div>

<br>

<h2 align="center">📝 Fichiers inclus</h2>

<div align="center">
  <table>
    <tr>
      <td>📄 <code>Dockerfile</code></td>
      <td>Configuration Docker</td>
    </tr>
    <tr>
      <td>📄 <code>nginx.conf</code></td>
      <td>Configuration Nginx</td>
    </tr>
    <tr>
      <td>📄 <code>README.md</code></td>
      <td>Documentation</td>
    </tr>
  </table>
</div>

<br>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer">
  
  <img src="https://komarev.com/ghpvc/?username=WorldSolutionRdc&label=Vues+du+projet&color=blue&style=flat-square" alt="visitor badge">
  
  <br><br>
  
  <b>⭐ N'hésitez pas à laisser une étoile si ce projet vous est utile ! ⭐</b>
  
  <br><br>
  
  <b>Maintenu avec ❤️ par <a href="https://github.com/WorldSolutionRdc">WorldSolutionRdc</a></b>
  
  <br>
  
  <i>Dernière mise à jour : 4 jours ago</i>
</div>

</body>
</html>
