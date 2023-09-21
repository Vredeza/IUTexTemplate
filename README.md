# IUTexTemplate

Template [LaTeX](https://wikipedia.org/wiki/LaTeX) permettant l'export de fichiers Markdown en PDF correspondants à la [charte graphique de l'IUT de Montpellier-Sète](https://iut-montpellier-sete.edu.umontpellier.fr/files/2020/09/Charte-graphique-de-lIUTMS-Septembre-2020.pdf).

Résultats : 

![markdown](markdown.md)

![output](output.pdf)

## Pré-requis

- [Pandoc](https://pandoc.org/)
- Multiples packages LaTeX (à renseigner)
- LuaLaTeX ou XeLaTeX

## Utilisation

Après avoir récupéré [`IUTexTemplate`](IUTexTemplate.tex) et le dossier [`ressources/`](ressources) vous pouvez convertir votre fichier :

```bash
pandoc votre_fichier_markdown.md --pdf-engine=lualatex --template=IUTexTemplate -o output.pdf
```

