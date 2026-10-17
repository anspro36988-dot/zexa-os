# Zexa OS — SM-T520

ROM expérimentale Android 10 basée sur LineageOS 17.1 pour la Samsung Galaxy
Tab Pro 10.1 Wi-Fi **SM-T520 seulement** (`n2awifi` / `picassowifi`).

## État du projet

Les versions sont des personnalisations d'une base binaire communautaire ; elles
ne sont pas encore reconstruites entièrement depuis les sources. L'animation
ZEXA, le fond bleu et la préparation de l'Updater sont ajoutés lors de
l'installation. L'accueil Zexa ajoute un fond turquoise/anthracite, une grande
horloge et un dock rond. Choisir « Accueil Zexa » comme lanceur après installation.
Le verrouillage et les paramètres conservent leur interface d'origine.

**Aucun démarrage ou flash n'a été validé sur tablette réelle.** La base signale
un microphone défectueux et son correctif de sécurité date du 5 avril 2021.
Il ne s'agit pas d'une version stable ou recommandée pour un usage sensible.

## Distribution

Les ZIP de ROM doivent être téléchargés dans Releases. Le catalogue GitHub Pages
est prévu à `https://anspro36988-dot.github.io/zexa-os/n2awifi.json`.
L'activation de Pages et la disponibilité réelle des assets doivent être
vérifiées avant d'annoncer le service OTA actif.

La version 0.4 contient cette adresse et le certificat public Zexa. Pour passer
des versions 0.1 ou 0.2 à cette configuration, une installation initiale via
TWRP est nécessaire. Les mises à jour suivantes utilisent la même clé de signature.

## Contrôles

Le système de fichiers de la base a été parcouru : 2 850 fichiers et 142 APK,
sans erreur de lecture ou de CRC. Les tests hôte vérifient les signatures et
rejettent les paquets modifiés, tronqués, de mauvais modèle ou de mauvais signataire.
Ces tests ne remplacent pas les essais de RecoverySystem, TWRP et du matériel.

## Retour arrière

Restauration manuelle TWRP uniquement après sauvegarde cohérente de Boot, System
et Data sur microSD d'au moins 8 Go, avec un espace libre réellement suffisant.
Pas de retour arrière automatique ni de mécanisme A/B. Sans microSD, cette option
n'est pas proposée dans le périmètre actuel du projet.

## Origine et crédits

- Base binaire : https://archive.anarchy-droid.com/n2awifi/LineageOS-17.1/
- Sources matérielles de référence : https://github.com/exynos5420/android_device_samsung_n2awifi/tree/lineage-17.1
- Updater : https://github.com/LineageOS/android_packages_apps_Updater/tree/lineage-17.1

Les composants tiers conservent leurs licences. La correspondance reproductible
entre la base archivée et les sources matérielles n'a pas été établie. Aucun lien
d'affiliation avec Samsung ou l'équipe LineageOS n'est revendiqué.

## GApps

Installation facultative séparée : Open GApps ARM / Android 10 / pico, depuis https://opengapps.org/. Compatibilité à tester sur appareil, aucune certification Google annoncée. Voir GAPPS.md.
