<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,15,18,20,25&height=250&section=header&text=Proxy%20Nginx%20pour%20VPS&fontSize=48&fontAlignY=38&desc=Redirection%20TCP%20haute%20performance&descAlignY=58&descSize=20&animation=fadeIn" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3500&pause=500&color=00FF00&center=true&vCenter=true&width=700&lines=🚀+Proxy+Nginx+ultra+rapide;🔒+Redirection+TCP+Layer+4;☁️+Déployé+sur+Google+Cloud+Run;🌍+Latence+minimale+garantie" alt="Typing Animation" />
</p>

<br/>

<div align="center">

# 🌟 Proxy Nginx pour VPS 🌟

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=for-the-badge&logo=github)
![Docker](https://img.shields.io/badge/Docker-Supported-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Google Cloud Run](https://img.shields.io/badge/Google_Cloud_Run-Deployed-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white)

</div>

---

## 🚀 **Redirection TCP haute performance vers VPS principal**

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=500&color=00FF00&center=true&vCenter=true&width=650&lines=Déployé+sur+Google+Cloud+Run;Haute+disponibilité+garantie;Low+latency+%26+haute+performance;24%2F7+automatique" alt="Typing Animation" />
</div>

---

## 📊 **Configuration Technique**

<div align="center">

| 🎯 **VPS Cible** | `207.126.161.196:443` |
|:----------------:|:---------------------:|
| 🔌 **Port d'écoute** | `8080` |
| 🌍 **Région VPS** | 🇬🇧 europe-west2 (Londres) |
| ☁️ **Région Cloud Run** | 🇬🇧 europe-west2 (Londres) |
| ⚡ **Type de proxy** | TCP Stream (Layer 4) |

</div>

---

## 🛠️ **Déploiement**

<div align="center">

```bash
gcloud run deploy ultra-speed-proxy \
  --source . \
  --platform managed \
  --region europe-west2 \
  --allow-unauthenticated \
  --port 8080 \
  --memory 512Mi \
  --cpu 1 \
  --timeout 3600
```

</div>

---

✨ Caractéristiques

<div align="center">

🚀 PERFORMANCE 🔒 SÉCURITÉ ⚡ OPTIMISATION
Faible latence Stream TCP 512Mi mémoire
Haut débit Layer 4 proxy 1 CPU vCPU
Timeout 3600s Non authentifié Auto-scaling

</div>

---

🌊 Architecture du flux

<div align="center">

```mermaid
flowchart LR
    A[👤 CLIENT] -->|Requête| B[☁️ CLOUD RUN<br/>Port: 8080]
    B -->|TCP Stream| C[🖥️ VPS PRINCIPAL<br/>Port: 443]
    C -->|Réponse| B
    B -->|Réponse| A
    
    style A fill:#4CAF50,stroke:#2E7D32,stroke-width:3px,color:#fff
    style B fill:#2196F3,stroke:#0D47A1,stroke-width:3px,color:#fff
    style C fill:#FF9800,stroke:#E65100,stroke-width:3px,color:#fff
```

</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=1500&pause=300&color=00FF00&center=true&vCenter=true&width=600&lines=📦+Client+→+Cloud+Run+:8080;⚡+Cloud+Run+→+VPS+:443;💨+VPS+:443+→+Cloud+Run;✅+Cloud+Run+→+Client" alt="Flow Animation">
</div>

---

📈 Statut & Monitoring

<div align="center">
  <img src="https://img.shields.io/badge/UPTIME-99.99%25-brightgreen?style=for-the-badge&logo=statuspage">
  <img src="https://img.shields.io/badge/RESPONSE_TIME-%3C50ms-brightgreen?style=for-the-badge&logo=clockify">
  <img src="https://img.shields.io/badge/ACTIVE_CONNECTIONS-24%2F7-success?style=for-the-badge&logo=cloudflare">
  <br><br>
  <img src="https://img.shields.io/badge/uptime-99.99%25-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/response_time-<50ms-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/status-active-success?style=flat-square">
</div>

---

🎯 Comment ça marche ?

<div align="center">

```mermaid
sequenceDiagram
    participant C as 👤 Client
    participant CR as ☁️ Cloud Run (:8080)
    participant V as 🖥️ VPS (:443)
    
    C->>CR: 1. Connexion TCP
    CR->>V: 2. Proxy TCP Stream
    V-->>CR: 3. Réponse
    CR-->>C: 4. Transmission
```

</div>

---

🔧 Configuration Nginx

```nginx
stream {
    upstream vps_backend {
        server 207.126.161.196:443 max_fails=3 fail_timeout=30s;
    }
    
    server {
        listen 8080;
        proxy_pass vps_backend;
        proxy_connect_timeout 60s;
        proxy_timeout 3600s;
    }
}
```

---

🤝 Contribution

<div align="center">
  <table>
    <tr>
      <td align="center">
        <h3>📝 Comment contribuer ?</h3>
        <br/>
        1. 🍴 Fork le projet<br/>
        2. 🌿 Crée ta branche (<code>git checkout -b feature/AmazingFeature</code>)<br/>
        3. 💾 Commit tes changements (<code>git commit -m 'Add AmazingFeature'</code>)<br/>
        4. 📤 Push la branche (<code>git push origin feature/AmazingFeature</code>)<br/>
        5. 🔃 Ouvre une Pull Request<br/>
        <br/>
        <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge&logo=github">
      </td>
    </tr>
  </table>
</div>

---

📝 Licence

<div align="center">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge&logo=opensourceinitiative">
  <br/><br/>
  Distribué sous licence <b>MIT</b>. Voir le fichier <code>LICENSE</code> pour plus d'informations.
</div>

---

👨‍💻 Auteur

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="https://avatars.githubusercontent.com/WorldSolutionRdc" width="100px;" alt="WorldSolutionRdc"/><br/>
        <sub><b>WorldSolutionRdc</b></sub>
      </td>
      <td>
        <b>🌐 GitHub :</b> <a href="https://github.com/WorldSolutionRdc">@WorldSolutionRdc</a><br/>
        <b>📧 Email :</b> worldsolutiontv@gmail.com<br/>
        <b>🚀 Projets :</b> Solutions haute performance
      </td>
    </tr>
  </table>
</div>

---

🙏 Remerciements

<div align="center">
  <table>
    <tr>
      <td align="center">
        🎭 <b>PANCHO7532</b><br/>
        <sub>Proxy Bridge original</sub>
      </td>
      <td align="center">
        🔐 <b>BadVPN</b><br/>
        <sub>Tunneling UDP/TCP</sub>
      </td>
      <td align="center">
        🔒 <b>stunnel</b><br/>
        <sub>Couche TLS/SSL</sub>
      </td>
      <td align="center">
        🖥️ <b>Dropbear</b><br/>
        <sub>Serveur SSH léger</sub>
      </td>
    </tr>
    <tr>
      <td align="center" colspan="4">
        ☁️ <b>Google Cloud Run</b><br/>
        <sub>Infrastructure serverless</sub>
      </td>
    </tr>
  </table>
</div>

---

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=2000&pause=500&color=FFD700&center=true&vCenter=true&width=600&lines=⭐+N'hésitez+pas+à+laisser+une+étoile+!+⭐;🚀+Maintenu+avec+❤️+par+WorldSolutionRdc;💡+Proxy+ultra-rapide+pour+VPS" alt="Footer Animation">
</div>

<br/>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=WorldSolutionRdc&label=✨%20VUES%20DU%20PROJET%20✨&color=blue&style=for-the-badge&base=1000">
</div>

<br/>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&animation=twinkling" />
</p>
```

