# Préparer le dépôt Zenodo

Les métadonnées proposées pour l’édition v1.1 sont dans `.zenodo.json`. Le
fichier `CITATION.cff` fournit aussi une citation à GitHub. Quand les deux
fichiers sont présents, Zenodo indique qu’il utilise `.zenodo.json` pour
l’archivage GitHub et ignore `CITATION.cff`; GitHub peut néanmoins afficher la
citation CFF.

## Avant le dépôt

- Relire le nom d’auteur affiché (`Ghaïs`) et les métadonnées du dépôt.
- Vérifier que le contenu à archiver correspond au tag Git local `v1.1`.
- Garder le dépôt privé tant que la publication n’est pas décidée.
- Ne pas sélectionner de licence open source : cette documentation est tous
  droits réservés.
- Pour une mise en ligne publique sur Zenodo, choisir explicitement les droits
  d’accès et les conditions de réutilisation au moment de créer le dépôt.

## Limite de l’intégration GitHub

L’intégration GitHub de Zenodo ne peut pas archiver un dépôt privé. Elle ne
doit donc pas être activée en attendant de rendre le dépôt accessible. Une fois
le dépôt public, l’archivage automatique peut suivre un release GitHub. Sinon,
les mêmes fichiers peuvent être déposés manuellement dans Zenodo depuis le
compte du titulaire.

Aucun dépôt Zenodo, DOI ou release hébergé n’a été créé par cette préparation.
Le DOI est attribué par Zenodo lors de la publication de l’enregistrement;
laisser ce champ absent jusque-là.
