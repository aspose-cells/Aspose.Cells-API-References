---
title: set_header méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 200
url: /fr/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
Définit un script mettant en forme l'en-tête d'un fichier Excel.



```python
def set_header(self, section, header_script):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| section | int | : Section gauche, 1 : Section centrale, 2 : Section droite.|
| header_script | str | Script de format d'en-tête.|
###  Remarques

Commandes de script :

| Commande| Description|
| :- | :- |
| &P| Numéro de la page actuelle|
| &N| Nombre de pages|
| &D| Date actuelle|
| &T| Heure actuelle|
| &UN| Nom de la feuille|
| &F| Nom de fichier sans chemin|
| &"<FontName>"| Nom de la police, par exemple : &"Arial"|
| &"<FontName>, <FontStyle>"| Nom et style de police, par exemple : &"Arial,Gras"|
| &<FontSize>| Taille de police. Si cette commande est suivie d'un nombre en clair à imprimer dans l'en-tête, il sera séparé de la hauteur de la police par un espace.|
| &K<RRGGBB>| Couleur de la police, par exemple (RED) : &KFF0000|
| &G| Script d'image|

Par exemple : "&Arial,Bold&8Header Note"


###  Voir également
* module [aspose.cells](../../)
* classe [PageSetup](/cells/fr/python-net/aspose.cells/pagesetup)
