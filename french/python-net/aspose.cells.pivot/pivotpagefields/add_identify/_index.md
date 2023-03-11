---
title: add_identify méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Définit l'étiquette d'élément dans chaque champ de page à utiliser pour identifier la plage de données.
Le pageItemIndex.Length doit être égal à PageFieldCount, donc veuillez d'abord ajouter le champ de page.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| range_index | int |Index de plage de données de consolidation.|
| page_item_index | list | L'index de l'élément de page dans chaque champ de page.<br/>pageItemIndex[2] = 1 signifie le deuxième élément du troisième champ à utiliser pour identifier cette plage.<br/> pageItemIndex[1] = -1 signifie aucun élément dans le deuxième champ à utiliser pour identifier cette plage<br/> et MS créera automatiquement un élément "vide" dans le deuxième champ pour identifier cette plage.|



###  Voir également
* module [aspose.cells.pivot](../../)
* classe [PivotPageFields](/cells/fr/python-net/aspose.cells.pivot/pivotpagefields)
