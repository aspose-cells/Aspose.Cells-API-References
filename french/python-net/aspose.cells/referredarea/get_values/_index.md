---
title: get_values méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/referredarea/get_values/
is_root: false
---
##  get_values() {#}
Obtient les valeurs des cellules dans cette zone.


###  Retour

Si cette zone est invalide, "#REF!" sera retourné ;
Si cette zone est une seule cellule, renvoyez l'objet de valeur de cellule ;
Sinon, renvoyez un tableau 2D pour toutes les valeurs de cette zone.


```python
def get_values(self):
    ...
```




##  get_values(calculate_formulas) {#bool}
Obtient les valeurs des cellules dans cette zone.


###  Retour

Si cette zone est invalide, "#REF!" sera retourné ;
Si cette zone est une seule cellule, renvoyez l'objet de valeur de cellule ;
Sinon, renvoyez un tableau 2D pour toutes les valeurs de cette zone.


```python
def get_values(self, calculate_formulas):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| calculate_formulas | bool | Dans cette plage, s'il y a des formules qui n'ont pas été calculées,<br/> ce drapeau indique si ces formules doivent être calculées de manière récursive|



###  Voir également
* module [aspose.cells](../../)
* classe [ReferredArea](/cells/fr/python-net/aspose.cells/referredarea)
