# 💣 Demineur

**Le classique du deminage, revisite avec Pygame.**

> Clic gauche pour reveler. Clic droit pour flagger. Ne saute pas.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pygame](https://img.shields.io/badge/Pygame-green?style=flat&logo=python&logoColor=white)

---

## Fonctionnalites

- **Grille 8x8** avec mines aleatoires
- **Revelation recursive** — clic sur une case vide revele automatiquement les cases adjacentes
- **Drapeaux** — clic droit pour marquer les mines suspectees
- **Compteur de mines** — affichage du nombre de mines autour de chaque case
- **Detection de victoire** — le jeu detecte quand toutes les cases sures sont revelees
- **Game over visuel** — les mines se revelent en rouge a la defaite

## Lancement

```bash
# Pre-requis
pip install pygame

# Jouer
python demineur.py
```

## Controles

| Action | Input |
|--------|-------|
| Reveler une case | Clic gauche |
| Poser/retirer un drapeau | Clic droit |

## Stack technique

- **Python 3** + **Pygame** pour le rendu graphique
- Grille generee aleatoirement a chaque partie
- Algorithme de flood-fill pour la revelation en cascade

---

*Un classique. Simple. Addictif. Explosif.*
