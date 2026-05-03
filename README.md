# 🌿 Mon Jardin d'Intérieur

> Site statique de suivi et d'entretien pour ma collection de plantes d'intérieur — hébergé sur GitHub Pages.

<br>

## 🪴 La collection

| Plante | Nom scientifique | Famille | Arrosage (P/É) |
|--------|-----------------|---------|----------------|
| 🍃 Lierre commun | *Hedera helix* | Araliaceae | 1× / semaine |
| 🌴 Kentia Palm | *Howea forsteriana* | Arecaceae | 1× / semaine |
| ☕ Composition tasse | *Ophiopogon + Pilea glauca* | — | 2–3 cuillères / semaine |
| 🎋 Bonsaï Ligustrum | *Ligustrum sinense* | Oleaceae | Quotidien en été |
| 🌵 Echeveria | *Echeveria elegans* | Crassulacées | 1× / 2 semaines |

<br>

## ✨ Fonctionnalités

- **Page d'accueil** avec présentation de toutes les plantes et liens rapides vers chaque fiche
- **Suivi d'arrosage dynamique** — calcule automatiquement quelles plantes arroser aujourd'hui selon la date et la saison (printemps/été vs automne/hiver), sans aucun serveur
- **Mémorisation locale** — cocher ✅ une plante comme arrosée enregistre la date dans le navigateur (`localStorage`) et recalcule les prochains arrosages
- **Fiches détaillées** pour chaque plante : état de santé, luminosité, arrosage, substrat, fertilisation, taille, signes de faiblesse et conseils saisonniers
- **100% responsive** — optimisé mobile, tablette et desktop
- **Zéro dépendance** — HTML, CSS, JavaScript vanilla, aucun framework

<br>

## 📁 Structure

```
FichePlante/
├── index.html                  # Page d'accueil + suivi d'arrosage
├── fiche_lierre.html            # Hedera helix
├── fiche_kentia.html            # Howea forsteriana
├── fiche_composition.html       # Ophiopogon + Pilea glauca
├── fiche_bonsai_ligustrum.html  # Ligustrum sinense
├── fiche_echeveria.html         # Echeveria elegans
└── README.md
```

<br>

## 🚀 Déploiement (GitHub Pages)

1. Aller dans **Settings → Pages**
2. Source : branche `main`, dossier `/root`
3. Sauvegarder — le site sera disponible à :

```
https://edward-nl.github.io/FichePlante/
```

<br>

## 💧 Comment fonctionne le suivi d'arrosage

Le tracker est entièrement statique — aucun serveur, aucune base de données.

- La **date du jour** est lue via `new Date()` dans le navigateur
- La **saison** est détectée automatiquement (avril–septembre = printemps/été)
- Chaque plante a une **fréquence d'arrosage en jours** selon la saison
- La **dernière date d'arrosage** est stockée dans `localStorage` sous la clé `watered_<id>`
- Une carte passe en **vert** (à arroser aujourd'hui), **orange** (dans 2 jours) ou **gris** (pas besoin)
- Cliquer le bouton ✅ marque la plante comme arrosée et réinitialise le compte

> Les données persistent entre les sessions sur le même navigateur. En naviguant depuis un autre appareil, le compteur repart de zéro.

<br>

## 🗓️ Calendrier d'arrosage

| Plante | Printemps · Été | Automne · Hiver |
|--------|----------------|----------------|
| 🍃 Lierre | 1× / 7 jours | 1× / 12 jours |
| 🌴 Kentia | 1× / 7 jours | 1× / 14 jours |
| ☕ Composition | Très léger / semaine | Très léger / semaine |
| 🎋 Bonsaï | Quotidien | 1–2× / semaine |
| 🌵 Echeveria | 1× / 14 jours | 1× / 30 jours |

<br>

## 🌱 Conseils du mois de Mai

- ✂️ **Tailler** le Lierre et le Bonsaï — meilleure période de l'année
- 🏺 **Rempoter** l'Echeveria (substrat inadapté) et la Composition (trop petite)
- 🌱 **Reprendre la fertilisation** mensuelle pour toutes les plantes
- ☀️ **Sortir** l'Echeveria et le Bonsaï en extérieur à partir de mi-mai
- 🐛 **Surveiller** les araignées rouges avec le retour de la chaleur (Lierre, Bonsaï)

<br>

---

*Fiches générées le 03/05/2026 · Raismes, Hauts-de-France 🇫🇷*
