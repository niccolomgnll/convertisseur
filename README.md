# Convertisseur

Outil web en une seule page pour préparer les fichiers CSV de l'équipe e-commerce :

- **Flux CSV** : change le séparateur d'un CSV (virgule, point-virgule, pipe, tabulation…) sans casser les descriptions qui contiennent des virgules, des guillemets ou des retours à la ligne. Séparateur et encodage source détectés automatiquement.
- **Nos-marques** : convertit le catalogue marques Excel au format Wishibam (CSV virgule, UTF-8 avec BOM). Bloque l'export en cas de doublon et signale les marques sans emplacement magasin.
- **Exports OMS** : nettoie `export_orders` / `export_line_items`, ou les fusionne sur `id_external`.

## Utilisation

Ouvrir l'adresse GitHub Pages du dépôt, déposer un fichier, télécharger le résultat.

Les fichiers sont traités entièrement dans le navigateur : aucune donnée n'est envoyée à un serveur.

## Technique

- Un seul fichier `index.html`, sans installation.
- Lecture Excel : SheetJS Community Edition 0.18.5 (Apache-2.0), intégrée au fichier.
