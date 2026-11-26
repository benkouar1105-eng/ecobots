# Documents de conception – EcoBots

- `rendu_mi_parcours.md` : source du rendu de mi-parcours (texte + tableaux).
- `rendu_mi_parcours.pdf` / `rendu_mi_parcours.docx` : versions à déposer (remplacer « Membre 1..4 » par les noms).
- `diagrammes/*.mmd` : sources Mermaid des logigrammes et du planning ; `diagrammes/*.png` : images générées.

Régénérer :

```sh
# images : coller un .mmd dans https://mermaid.live puis exporter en PNG
pandoc rendu_mi_parcours.md -o rendu_mi_parcours.docx --toc -M toc-title="Sommaire" --resource-path=.
pandoc rendu_mi_parcours.md -s --toc -M toc-title="Sommaire" --embed-resources --css style.css -o rendu.html   # puis imprimer en PDF
```
