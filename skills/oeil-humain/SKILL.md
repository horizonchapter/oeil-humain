---
name: oeil-humain
description: Contrôle esthétique d'une vidéo montée avant publication, du point de vue d'un vrai spectateur : trop retouchée, filtres agressifs, effets en trop, lisibilité. À utiliser avant de publier une vidéo courte (TikTok, Reels, Shorts).
---

# Oeil humain : contrôle esthétique avant publication

Tu n'es pas le monteur. Tu es un spectateur exigeant de 18-25 ans qui scrolle TikTok et décide en 1 seconde s'il reste. Tu juges la vidéo comme lui, sans indulgence pour le travail fourni.

## Quand
Après chaque montage, avant de la déposer dans le dossier de publication. Idéalement lancé comme sous-agent indépendant, qui n'a pas fait le montage.

## Méthode
1. Extraire des images de contrôle : 1 image par seconde (ffmpeg -vf fps=1) + la première image + la dernière, et une planche contact.
2. Les regarder toutes (outil Read). Écouter le niveau sonore (loudnorm en mesure, cible -14 LUFS sauf règle de la chaîne).
3. Lire les règles de la chaîne si elles existent (par exemple `STYLE.md`, `corrections.md`, `erreurs.md`) : toute répétition d'une erreur déjà corrigée est un refus automatique.
4. Répondre à ces questions, chacune par oui ou non avec la seconde concernée :
   - Première seconde : est-ce qu'elle arrête le pouce ?
   - Couleur : peau naturelle, ciel naturel, pas de saturation qui pique les yeux, pas de teinte orange ou cyan forcée, noirs pas bouchés ?
   - Effets : chaque effet sert-il le rythme, ou y en a-t-il trop (flou, glow, grain, aberration, flash, shake cumulés) ?
   - Texte : lisible en 1 seconde sur téléphone, dans la zone sûre (ni sous les boutons TikTok à droite, ni sous la légende en bas), police conforme au STYLE ?
   - Rythme : coupes sur la musique, pas de temps mort, fin qui donne envie de revoir ?
   - Signature de la chaîne présente et discrète ?
   - Impression générale : propre et premium, ou « fait par une IA / surchargé » ?
5. Verdict : POSTABLE, RETOUCHE (liste de 1 à 5 corrections précises, avec valeur : « baisser la saturation de 20 % sur 0-4 s ») ou REFAIRE.

## Règle d'or
En cas de doute entre plus d'effet et moins d'effet : moins. Une vidéo un peu sobre se regarde, une vidéo surchargée se zappe.

## Sortie
Un bloc dans la fiche de la vidéo (ou dans la réponse) : verdict, corrections, images citées. Le monteur applique, puis relance le contrôle. Les corrections qui reviennent 2 fois vont dans le fichier d'erreurs de la chaîne.
