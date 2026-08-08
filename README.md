<div align="center">

<img width="64" height="64" alt="Logo Student_Record_Manager" src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCI+CiAgPHJlY3Qgd2lkdGg9IjY0IiBoZWlnaHQ9IjY0IiByeD0iMTYiIGZpbGw9IiMxQjE4MTUiLz4KICA8cG9seWdvbiBwb2ludHM9IjI2LDE1IDM4LDI1IDI2LDM1IDE0LDI1IiBmaWxsPSIjQjg3RjRFIiBzdHJva2U9IiM4QzVGMzciIHN0cm9rZS13aWR0aD0iMS41IiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8+CiAgPHJlY3QgeD0iMjQiIHk9IjM1IiB3aWR0aD0iNCIgaGVpZ2h0PSI2IiByeD0iMS41IiBmaWxsPSIjOEM1RjM3Ii8+CiAgPHBhdGggZD0iTTM4IDI1IEg0OCBWNDEgSDU0IiBmaWxsPSJub25lIiBzdHJva2U9IiNGM0VDRTEiIHN0cm9rZS13aWR0aD0iMi40IiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz4KICA8Y2lyY2xlIGN4PSI0OCIgY3k9IjMzIiByPSIxLjgiIGZpbGw9IiNGM0VDRTEiLz4KICA8Y2lyY2xlIGN4PSI1NCIgY3k9IjQxIiByPSIzLjIiIGZpbGw9IiNGM0VDRTEiLz4KICA8Y2lyY2xlIGN4PSI1NCIgY3k9IjQxIiByPSIxLjIiIGZpbGw9IiMxQjE4MTUiLz4KPC9zdmc+Cg==" />

# Student_Record_Manager

**Registre de classe** — suivez les notes, le statut et la progression de vos étudiants, et générez le bulletin de classe en un instant.

![HTML5](https://img.shields.io/badge/HTML5-1B1815?style=for-the-badge&logo=html5&logoColor=F3ECE1)
![CSS3](https://img.shields.io/badge/CSS3-B87F4E?style=for-the-badge&logo=css3&logoColor=1B1815)
![JavaScript](https://img.shields.io/badge/JavaScript-6B7A5E?style=for-the-badge&logo=javascript&logoColor=F3ECE1)
![No dependencies](https://img.shields.io/badge/Dépendances-aucune-A85B3C?style=for-the-badge)

</div>

---

## Aperçu

**Student_Record_Manager** est un mini-site autonome (HTML / CSS / JS, sans framework ni backend) pour gérer un registre d'étudiants : ajout, modification de note, suppression, recherche, tri, et un bulletin de classe généré automatiquement avec un graphique de répartition des notes.

Les données sont conservées dans le navigateur (`localStorage`) : elles persistent d'une visite à l'autre, sans base de données.

## Fonctionnalités

- 📋 **Fiches étudiants** : nom, âge, statut (actif/inactif), note sur 20
- 🔍 **Recherche** par nom, **filtre** par statut, **tri** (note ↑/↓, nom A→Z)
- ➕ **Ajout** d'un étudiant avec validation des champs
- ✏️ **Modification de note** via une fenêtre de confirmation dédiée
- 🗑️ **Suppression** avec confirmation
- ♻️ **Réinitialisation** aux données de démonstration
- 🧾 **Bulletin de classe** : moyenne, meilleur/pire étudiant, taux de réussite
- 📊 **Graphique** de répartition des notes par étudiant
- 🖨️ **Impression** du bulletin en un clic
- 💾 **Sauvegarde automatique** locale (`localStorage`)

## Palette de couleurs

Le thème s'inspire d'un intérieur chaleureux — crème, noir profond, terracotta — décliné dans toute l'interface (boutons, tampons de notes, badges de statut, graphiques).

| Couleur | Usage | Code |
|---|---|---|
| <img src="https://placehold.co/16x16/1B1815/1B1815.png" width="16" height="16" /> Noir profond | Header, boutons principaux, texte du hero | `#1B1815` |
| <img src="https://placehold.co/16x16/2E2822/2E2822.png" width="16" height="16" /> Brun foncé | Dégradé du hero | `#2E2822` |
| <img src="https://placehold.co/16x16/F3ECE1/F3ECE1.png" width="16" height="16" /> Crème | Fond de page | `#F3ECE1` |
| <img src="https://placehold.co/16x16/FBF7F0/FBF7F0.png" width="16" height="16" /> Blanc cassé | Fond des cartes | `#FBF7F0` |
| <img src="https://placehold.co/16x16/221E1A/221E1A.png" width="16" height="16" /> Encre | Texte principal | `#221E1A` |
| <img src="https://placehold.co/16x16/8A7F70/8A7F70.png" width="16" height="16" /> Taupe | Texte secondaire | `#8A7F70` |
| <img src="https://placehold.co/16x16/E3D9C8/E3D9C8.png" width="16" height="16" /> Beige clair | Bordures, séparateurs | `#E3D9C8` |
| <img src="https://placehold.co/16x16/B87F4E/B87F4E.png" width="16" height="16" /> Terracotta | Accent principal, tampon de réussite | `#B87F4E` |
| <img src="https://placehold.co/16x16/6B7A5E/6B7A5E.png" width="16" height="16" /> Sauge | Statut "réussi" / "actif" | `#6B7A5E` |
| <img src="https://placehold.co/16x16/A85B3C/A85B3C.png" width="16" height="16" /> Rouille | Statut "échoué", suppression | `#A85B3C` |

Ces couleurs sont définies comme variables CSS dans `:root` (`style.css`), donc modifiables en un seul endroit.

**Typographies :** [Fraunces](https://fonts.google.com/specimen/Fraunces) (titres) · [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans) (texte courant) · [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) (chiffres, identifiants)

## Structure du projet

```
Student_Record_Manager/
├── index.html   → structure de la page
├── style.css    → thème visuel (couleurs, mise en page, animations, impression)
├── script.js    → données et logique (CRUD étudiants, bulletin, graphique)
└── README.md    → ce fichier
```

## Démarrage rapide

Aucune installation requise.

1. Garder les trois fichiers (`index.html`, `style.css`, `script.js`) dans le **même dossier**.
2. Ouvrir `index.html` dans un navigateur.

C'est tout — le site fonctionne entièrement côté client.

## Logique métier (`script.js`)

| Fonction | Rôle |
|---|---|
| `calculateAverageGrade(students)` | Moyenne générale de la classe |
| `findBestStudent(students)` / `findLowestStudent(students)` | Meilleur / plus faible étudiant |
| `hasPassed(student)` | `true` si la note ≥ 10 |
| `countPassedStudents` / `countFailedStudents` / `countActiveStudents` | Compteurs pour le bulletin |
| `isValidStudent(student)` | Validation des champs avant ajout |
| `addStudent` / `updateStudentGrade` / `removeStudentById` | Opérations CRUD sur le registre |
| `generateClassReport(students)` | Assemble toutes les statistiques du bulletin |

Les données sont automatiquement sauvegardées (`saveStudents()`) dans `localStorage` après chaque modification, et rechargées (`loadStudents()`) à l'ouverture du site.

## Personnalisation

- **Couleurs** : modifier les variables dans `:root` en haut de `style.css`.
- **Données de démonstration** : modifier le tableau `DEFAULT_STUDENTS` dans `script.js`.
- **Logo** : icône SVG intégrée directement dans `index.html` (header et pied de page) — facilement remplaçable par un autre SVG.

## Licence

Projet libre d'utilisation et de modification dans le cadre de votre usage personnel ou pédagogique.
