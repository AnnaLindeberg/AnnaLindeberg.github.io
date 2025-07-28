---
---

# Publications

## Published in peer-reviewed journal

{% bibliography --file published.bib -q @*[status!=submitted] %}

## Submitted

{% bibliography --file published.bib -q @*[status!=accepted] %}

## Others

{% bibliography --file other.bib --template otherbib%}