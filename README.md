# Analyseur de Trames Réseau

Un outil d’analyse et de diagnostic réseau permettant de capturer, visualiser et inspecter les trames circulant sur une interface réseau Windows.

Ce projet illustre l’utilisation des **RAW Sockets** via **WinSock 2** pour intercepter les paquets IP, et les analyser en détails (en-têtes, protocoles, ports, données brutes…).

⚠️ **Important :** Cet outil doit être utilisé **uniquement sur un réseau dont vous êtes propriétaire ou autorisé à administrer**.  
Il est conçu pour l’audit, la supervision, la formation et le diagnostic interne.

---

## 🚀 Fonctionnalités

### 🔍 Capture des trames
- Sélection de l’interface réseau
- Définition du nombre maximum de trames à capturer
- Capture en temps réel via RAW Sockets

### 📊 Tableau de visualisation
Chaque trame affichée contient :
- Numéro d’ordre  
- Durée depuis le début de la capture  
- Protocole (TCP / UDP / ICMP / IGMP)  
- IP source / destination  
- Ports source / destination  

### 🧩 Analyse détaillée
Dans le panneau de droite, chaque trame montre :
- En-tête IP (Version, TTL, checksum…)  
- En-tête TCP ou UDP (ports, flags, séquence…)  
- Données brutes en hexadécimal + représentation ASCII  

<img width="1366" height="720" alt="Capture d&#39;écran 2025-12-05 180635" src="https://github.com/user-attachments/assets/a7595f25-cb42-4bea-a981-9db90ceb3e44" />

### 🎛️ Filtrage avancé
Une fenêtre dédiée permet :
- Activation/désactivation de certains protocoles (IGMP, ICMP, UDP, TCP)  
- Filtrage par ports autorisés (TCP/UDP)  
- Filtrage multi-ports via `;` (ex : `80;443;21`)
  
<img width="426" height="203" alt="Capture d&#39;écran 2025-12-05 180653" src="https://github.com/user-attachments/assets/a39f7d35-7b91-4941-9c44-38b9265aee8c" />

### 📨 Messagerie
Une section didactique explique :
- Comment les applications réseau fonctionnent  
- Comment les trames circulent  
- Comment les administrateurs diagnostiquent un service (mail, FTP, …)  

<img width="403" height="420" alt="Capture d&#39;écran 2025-12-05 180730" src="https://github.com/user-attachments/assets/e5148bd8-e012-4cc1-a2c8-84979288584e" />

---

## 🖼️ Aperçu de l’interface

### Vue principale  
Affichage en temps réel de la capture :
- Liste des trames  
- Analyse complète  
- Vue hexadécimale des données  

*(Voir images ci-dessus dans le repository)*

### Module de filtrage  
Permet de réduire les trames visibles selon vos besoins.

### Module didactique  
Explication simplifiée du fonctionnement des échanges réseau.

---

## 🏗️ Technologies utilisées
- **WinSock 2 (RAW Sockets)**
- **WinDev**
- API Windows  
- Interface utilisateur Windows

