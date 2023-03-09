---
title: set_footer méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Définit un script mettant en forme le pied de page d'un fichier Excel.



```python
def set_footer(self, section, footer_script):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| section | int | : Section gauche, 1 : Section centrale, 2 : Section droite.|
| footer_script | str | Script de format de pied de page.|
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

Par exemple : "&Arial,Gras&Note de 8 pieds de page"


###  Voir également
* module [aspose.cells](../../)
* classe [PageSetup](/cells/fr/python-net/aspose.cells/pagesetup)
