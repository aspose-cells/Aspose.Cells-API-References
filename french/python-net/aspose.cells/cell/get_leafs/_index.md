---
title: get_leafs méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 160
url: /fr/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Obtenez toutes les cellules qui font directement référence à cette cellule et doivent être mises à jour lorsque cette cellule est modifiée.


###  Retour

Recenseur pour recenser toutes les personnes à charge (Cell)


```python
def get_leafs(self):
    ...
```


###  Remarques

REMARQUE : Cette classe est désormais obsolète.
veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir toutes les personnes à charge dans la chaîne de calcul.
Cette propriété sera supprimée 12 mois plus tard depuis mai 2022.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.

##  get_leafs(recursive) {#bool}
Obtenir toutes les cellules qui seront mises à jour lorsque cette cellule sera modifiée.


###  Retour

Recenseur pour recenser toutes les personnes à charge (Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| recursive | bool | Si renvoie les feuilles qui ne font pas directement référence à cette cellule<br/> mais référence à d'autres feuilles de cette cellule|
###  Remarques

REMARQUE : Cette classe est désormais obsolète.
veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir toutes les personnes à charge dans la chaîne de calcul.
Cette propriété sera supprimée 12 mois plus tard depuis mai 2022.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.


###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
