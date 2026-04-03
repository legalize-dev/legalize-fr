# Legalize — France

> **Early stage** — This repository is under active development. File structure, commit history, and content may undergo significant changes, including full regeneration. Do not build tooling against the current layout without expecting breaking changes.
>
> **Phase initiale** — Ce dépôt est en cours de développement actif. La structure des fichiers, l'historique des commits et le contenu peuvent subir des modifications importantes, y compris une régénération complète. Ne construisez pas d'outils basés sur la structure actuelle sans vous attendre à des changements incompatibles.

Législation française consolidée en Markdown, versionnée avec Git.

Chaque loi est un fichier. Chaque réforme est un commit.

Partie du projet [Legalize](https://github.com/legalize-dev/legalize) · [legalize.dev](https://legalize.dev)

## Structure

```
fr/
  LEGITEXT000006069414.md    — Code de commerce
  LEGITEXT000006070721.md    — Code civil
  LEGITEXT000006071154.md    — Code de procédure pénale
  ...
```

Le type de texte (code, loi, ordonnance, décret) est indiqué dans le frontmatter YAML de chaque fichier, pas dans l'arborescence.

## Source

Données issues de la base [LEGI](https://www.data.gouv.fr/datasets/legi-codes-lois-et-reglements-consolides) (open data, licence ouverte Etalab 2.0), publiée par la [DILA](https://www.dila.premier-ministre.gouv.fr/).

## Format

Chaque fichier contient :

- **Frontmatter YAML** : métadonnées (titre, identifiant, date, état juridique)
- **Corps Markdown** : texte consolidé avec structure hiérarchique

Les commits utilisent la date historique de publication officielle au Journal Officiel.

## Licence

Les textes législatifs sont dans le domaine public. La structuration et le formatage sont sous licence [MIT](LICENSE).

---

Créé par [Enrique Lopez](https://enriquelopez.eu) · [legalize.dev](https://legalize.dev)
