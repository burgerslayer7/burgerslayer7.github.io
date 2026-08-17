# Pokefan Index

Le catalogue public servi à Pokefan Launcher est généré par GitHub Pages.

## Structure

- `_data/pokefan_base.json` : catalogue de base complet.
- `_data/pokefan_games/<id>.json` : surcharge individuelle d'un jeu. Si le fichier existe, il remplace entièrement l'entrée du même `id` dans le catalogue de base.
- `Pokefan-index/games.json` : fichier généré automatiquement par Jekyll et consommé par le launcher.
- `Pokefan-index/editor.html` : assistant web pour générer une surcharge sans écrire le JSON à la main.

## Modifier un jeu

1. Ouvrir `https://burgerslayer7.github.io/Pokefan-index/editor.html`.
2. Choisir le jeu et la méthode d'installation.
3. Modifier les champs puis cliquer sur **Générer la fiche**.
4. Cliquer sur **Copier JSON**.
5. Ouvrir **Créer la fiche sur GitHub** (ou **Éditer sur GitHub** si elle existe déjà), coller le JSON puis valider le commit.
6. GitHub Pages reconstruit automatiquement `Pokefan-index/games.json`.

## Méthodes d'installation

- `direct-zip` : téléchargement direct d'une archive ZIP, extraction et recherche de `executable`.
- `github-release` : dernière release GitHub, avec `repository` et `assetPattern`.
- `flatpak` : installation Flatpak sous Linux.
- `external` : page officielle externe lorsque l'installation ne peut pas être automatisée proprement.
- `manual` : rattachement d'une installation existante.

Les ROM commerciales, BIOS, clés ou autres contenus propriétaires ne doivent jamais être ajoutés à cet index.
