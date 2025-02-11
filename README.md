# Komponenten 2.0
E-sektionen inom TLTHs nya sångbok.


## Hur man bygger sångboken
I VSCode lägg till följande i ``settings.json`` för att köra LaTeX med XeLaTeX. Det kanske även kräver extensionen [latex-workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop). Om detta inte fungerar fråga någon kunning i att uppdatera sektionens styrdokument (typ kontaktor eller ordförande).
```
"latex-workshop.latex.tools": [{
"name": "latexmk",
"command": "latexmk",
"args": [
    "-xelatex",
    "-synctex=1",
    "-interaction=nonstopmode",
    "-file-line-error",
    "%DOC%"
]
}],
```
