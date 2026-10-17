# Zexa OS 0.4 — accueil et GApps

## Accueil

La ROM pour **SM-T520 uniquement** intègre Accueil Zexa : fond anthracite/turquoise, grande horloge, date, dock rond et tiroir d'applications. Appuyer sur Accueil et choisir « Accueil Zexa » comme lanceur permanent. Le lanceur d'origine reste disponible.

## Applications Google facultatives

La base inspectée est Android 10 / SDK 29 / ARM 32 bits (`armeabi-v7a`). Le paquet à évaluer est **Open GApps : ARM / 10.0 / pico**, depuis https://opengapps.org/. Pico fournit le minimum nécessaire à Google Play. Ne pas choisir ARM64.

Les GApps ne sont pas intégrées au ZIP Zexa et ne sont pas redistribuées dans ses Releases. Leur installation, la connexion Google, Play Store et la conservation lors d'une mise à jour ne sont pas encore validés sur cette tablette. La présence du support addon.d dans la base ne prouve pas son fonctionnement avec un paquet donné. Aucune certification Google ni compatibilité Play Integrity n'est annoncée.

Avant d'installer un paquet, suivre sa documentation officielle et vérifier l'espace système ainsi que les exigences de première installation. Une installation existante avec un compte Google ne doit pas être modifiée sans sauvegarde adaptée.

## État des essais

- APK du lanceur : compilation Java/DEX, manifeste, signature v1/v2/v3 et alignement validés.
- ROM 0.4 : CRC, signature RSA/SHA256, conservation du noyau et des blocs système de la base validés ; 12 tests OTA/catalogue réussis.
- Base : audit en lecture de 2 850 fichiers et 142 APK déjà effectué sans erreur CRC.
- Non réalisés : démarrage, installation TWRP, affichage du lanceur, Wi-Fi/caméra/audio, installation GApps, OTA de bout en bout et restauration.

**Version expérimentale, non validée sur appareil.** La base signale un microphone défectueux et utilise un correctif de sécurité du 5 avril 2021. Retour arrière uniquement manuel via une sauvegarde TWRP sur microSD d'au moins 8 Go avec assez d'espace libre ; aucun retour arrière automatique.
