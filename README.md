# Indice du Baromètre de Gouvernance Locale
### Local Governance Barometer Index

Outil d'évaluation de la gouvernance locale par les communautés, en **français** avec sous-titres en **malagasy** (italique).
Une seule page HTML, sans serveur ni installation.

## Ce que fait l'outil

- 5 piliers : Efficacité, État de droit, Redevabilité, Équité, Participation
- 22 sous-critères et 68 indicateurs
- Chaque indicateur est une question à choix multiple à 4 niveaux (0, 33, 67, 100 points)
- Calcul automatique : sous-critère → pilier → score global (sur 100)
- Onglet **Plan d'action** : les faiblesses (réponses à 0 ou 33) alimentent des actions avec cause, résultat attendu, responsable, partenaires, axe d'intervention, horizon, échéance, budget (Ar), priorité et statut ; suivi de l'avancement ; groupe technique de suivi et date de la prochaine mesure
- Bouton **Imprimer / PDF** : génère un rapport A4 (résumé, détail par pilier, plan d'action, zones de signature)
- Les réponses restent dans le navigateur de l'utilisateur (localStorage), rien n'est envoyé en ligne

## Utiliser

Ouvrir `index.html` dans un navigateur, ou publier avec GitHub Pages :

1. Dépôt GitHub → **Settings** → **Pages**
2. Source : **Deploy from a branch**, branche `main`, dossier `/ (root)`
3. L'adresse du site apparaît après quelques minutes

Pour le PDF : bouton **Imprimer / PDF**, puis choisir « Enregistrer au format PDF » comme imprimante.
Activer « Graphiques d'arrière-plan » dans les options d'impression pour afficher les barres de couleur.

## Sources du cadre

- Guide to the Good Governance Barometer, FHI 360 / USAID, 2015 (piliers et sous-critères)
- Brillantes, A. (2001), *Developing Indicators of Local Governance in the Philippines: Towards an "ISO" for LGUs*
- Manasan, Gonzales et Gaffud (1999), *Indicators of Good Governance: Developing an Index of Governance Quality at the LGU Level*

Les indicateurs marqués **ADP** ont été ajoutés ou reformulés pour compléter un pilier. Les niveaux de réponse et la traduction malagasy sont une première version : à valider avec chaque communauté.

## Adapter

Tout est dans `index.html`. Les indicateurs sont dans la variable `DATA` du script : chaque ligne contient le texte « français|malagasy », la source, et les quatre niveaux de réponse du plus faible au plus fort.
