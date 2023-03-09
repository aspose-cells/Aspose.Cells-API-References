---
title: is_gather_string méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Vérifie si la valeur de chaîne actuelle de la cellule doit être rassemblée dans un pool global.


###  Retour

true si la valeur de chaîne doit être rassemblée dans un pool global pour le fichier résultant.


```python
def is_gather_string(self):
    ...
```


###  Remarques

La collecte de valeurs de chaîne ne profitera que lorsqu'il existe de nombreuses valeurs de chaîne dupliquées pour les cellules fournies par cette implémentation.
Dans cette situation, la chaîne de collecte économisera beaucoup de mémoire et générera un fichier résultant plus petit.
S'il existe de nombreuses valeurs de chaîne pour les cellules fournies par LightCellsDataProvider mais que peu d'entre elles sont identiques,
la chaîne de collecte coûtera plus de mémoire et de temps et n'a aucun avantage pour le fichier résultant.


###  Voir également
* module [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/fr/python-net/aspose.cells/lightcellsdataprovider)
