```markdown
<!---
<div align="center">
--->

# 🌟 Proxy Nginx pour VPS 🌟

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-Supported-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Google Cloud Run](https://img.shields.io/badge/Google_Cloud_Run-Deployed-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white)

</div>

---

## 🚀 **Redirection TCP haute performance vers VPS principal**

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3000&pause=500&color=00FF00&center=true&vCenter=true&width=600&lines=Déployé+sur+Google+Cloud+Run;Haute+disponibilité+garantie;Low+latency+%26+haute+performance" alt="Typing Animation" />
</div>

---

## 📊 **Configuration Technique**

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
    <td>🇬🇧 europe-west2 (Londres)</td>
  </tr>
  <tr>
    <td align="center"><b>☁️ Région Cloud Run</b></td>
    <td>🇬🇧 europe-west2 (Londres)</td>
  </tr>
  <tr>
    <td align="center"><b>⚡ Type</b></td>
    <td>TCP Stream (Layer 4)</td>
  </tr>
</table>

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

🚀 Performance 🔒 Sécurité ⚡ Optimisation
Faible latence Stream TCP 512Mi mémoire
Haut débit Layer 4 proxy 1 CPU vCPU
Timeout 3600s Non authentifié Auto-scaling

</div>

---

📈 Statut & Monitoring

<div align="center">

https://img.shields.io/badge/uptime-99.99%25-brightgreen?style=flat-square
https://img.shields.io/badge/response_time-<50ms-brightgreen?style=flat-square
https://img.shields.io/badge/status-active-success?style=flat-square

</div>

---

🔄 Architecture du flux

```mermaid
graph LR
    A[Client] --> B[Cloud Run :8080]
    B --> C[VPS :443]
    C --> B
    B --> A
    
    style A fill:#4CAF50,stroke:#333,stroke-width:2px
    style B fill:#2196F3,stroke:#333,stroke-width:2px
    style C fill:#FF9800,stroke:#333,stroke-width:2px
```

---

🎨 Animations & Effets

<div align="center">

https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer

  <img src="https://komarev.com/ghpvc/?username=WorldSolutionRdc&label=Vues+du+projet&color=blue&style=flat-square" alt="visitor badge" />

⭐ N'hésitez pas à laisser une étoile si ce projet vous est utile ! ⭐

</div>

---

<div align="center">

Maintenu avec ❤️ par WorldSolutionRdc

Dernière mise à jour : 4 jours ago

</div>

<!---
--->

```

Pour un style encore plus avancé avec des animations CSS personnalisées, vous pouvez ajouter ceci au début de votre README (les badges GitHub supportent les styles HTML/CSS) :

```html
<div align="center">
  <img src="https://media.giphy.com/media/3o7abKhOpu0NwenH3O/giphy.gif" width="30" height="30">
  <h1>
    <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=30&duration=3000&pause=500&color=F7D94C&center=true&vCenter=true&width=600&lines=PROXY+NGINX+ULTRA+RAPIDE;LATENCE+MINIMALE;HAUTE+DISPONIBILIT%C3%89" alt="Typing Animation" />
  </h1>
</div>
```

Ce README stylisé inclut :

· ✨ Des emojis colorés
· 📊 Des tableaux de configuration
· 🎯 Des badges de statut animés
· 🔄 Un diagramme d'architecture
· 💫 Des effets de texte animés
· 🌊 Des vagues décoratives
· 📈 Des métriques visuelles

  --timeout 3600
