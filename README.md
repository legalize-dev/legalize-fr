# Legalize FR

### Législation française consolidée en Markdown, versionnée avec Git.

Chaque loi est un fichier. Chaque réforme est un commit.

**83 codes** · Source officielle LEGI/Légifrance

Partie du projet [Legalize](https://github.com/legalize-dev/legalize) · [legalize.dev](https://legalize.dev)

> **Phase initiale** — Ce dépôt est en cours de développement actif. La structure des fichiers, l'historique des commits et le contenu peuvent subir des modifications importantes, y compris une régénération complète.

## Démarrage rapide

```bash
# Cloner la législation française
git clone https://github.com/legalize-dev/legalize-fr.git

# Rechercher un article dans le Code civil
grep -A 5 "Article 1240" fr/LEGITEXT000006070721.md

# Historique des modifications d'un code
git log --oneline -- fr/LEGITEXT000006070721.md
```

## Structure

```
fr/
  LEGITEXT000006070721.md    — Code civil
  LEGITEXT000006069414.md    — Code de commerce
  LEGITEXT000006071154.md    — Code de procédure pénale
  LEGITEXT000006072050.md    — Code du travail
  ...                        — 83 codes consolidés
```

Le type de texte (code, loi, ordonnance, décret) est indiqué dans le frontmatter YAML de chaque fichier, pas dans l'arborescence.

## Format

Chaque fichier contient :

- **Frontmatter YAML** — métadonnées : titre, identifiant, date de publication, état juridique, type de texte, identifiant ELI
- **Corps Markdown** — texte consolidé avec structure hiérarchique (parties, livres, titres, chapitres, articles)

Les commits utilisent la date historique de publication officielle au Journal Officiel. Chaque commit inclut des trailers avec l'identifiant du texte et de la réforme, ce qui permet de reconstruire l'historique législatif complet avec `git log`.

## Source

Données issues de la base [LEGI](https://www.data.gouv.fr/datasets/legi-codes-lois-et-reglements-consolides) (open data, licence ouverte Etalab 2.0), publiée par la [DILA](https://www.dila.premier-ministre.gouv.fr/).

## Licence

Les textes législatifs sont dans le domaine public. La structuration et le formatage sont sous licence [MIT](LICENSE).

---

Créé par [Enrique Lopez](https://enriquelopez.eu) · [legalize.dev](https://legalize.dev)
