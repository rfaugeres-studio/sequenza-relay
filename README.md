# Sequenza Relay

Petit programme qui relie une **caméra IP (RTSP)** à **Sequenza Live** pour séquencer un match en direct
sur [www.sequenza-video.com](https://www.sequenza-video.com).

Un navigateur ne sait pas lire une caméra RTSP : Sequenza Relay s'y connecte sur l'ordinateur du match
(même réseau que la caméra) et transmet l'image à Sequenza. Rien n'est envoyé ailleurs ; le mot de passe
de la caméra reste sur cet ordinateur.

## Télécharger

| Ordinateur | Fichier |
|---|---|
| Windows 10 / 11 | [Sequenza-Relay-windows.zip](Sequenza-Relay-windows.zip) |
| Mac à puce Apple (M1 à M4) | [Sequenza-Relay-mac-apple-silicon.tar.gz](Sequenza-Relay-mac-apple-silicon.tar.gz) |
| Mac à processeur Intel | [Sequenza-Relay-mac-intel.tar.gz](Sequenza-Relay-mac-intel.tar.gz) |

Empreintes SHA-256 : [SHA256SUMS.txt](SHA256SUMS.txt). Version 1.0.0.
Les versions Mac n'ont pas encore été essayées sur un Mac.

## Utiliser

1. Décompressez le fichier.
2. **Windows** : double-cliquez sur « Sequenza Relay.cmd ». Si Windows affiche « Windows a protégé votre
   ordinateur » (programme non signé) : « Informations complémentaires » › « Exécuter quand même ».
   **Mac** : clic droit sur « Sequenza Relay.command » › Ouvrir › Ouvrir (développeur non identifié :
   programme non signé).
3. Au premier lancement, MediaMTX est téléchargé automatiquement (une fois, empreinte vérifiée).
4. Laissez la fenêtre ouverte pendant le match, puis dans Sequenza : Sequenza Live › onglet « Caméra IP ».

Caméras H.265 : installez FFmpeg sur l'ordinateur pour la conversion en H.264.

## Composants

- [Node.js](https://nodejs.org) v24.22.1 (licence MIT), moteur officiel inclus tel quel.
- [MediaMTX](https://github.com/bluenviron/mediamtx) v1.21.2 (licence MIT), téléchargé au premier lancement.

© RF STUDIO — Sequenza.
