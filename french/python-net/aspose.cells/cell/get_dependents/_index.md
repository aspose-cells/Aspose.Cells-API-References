---
title: get_dependents méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Obtenez toutes les cellules dont la formule fait directement référence à cette cellule.



```python
def get_dependents(self, is_all):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| is_all | bool | Indique si vérifier les formules dans d'autres feuilles de calcul|
###  Remarques

* Si une référence contenant cette cellule apparaît dans la formule d'une cellule, cette cellule sera considérée comme

la personne à charge de cette cellule, peu importe la référence ou cette cellule est utilisée ou non lors du calcul.
Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
cette formule est toujours considérée comme dépendante de A2.
Pour obtenir les formules dont les résultats calculés dépendent de cette cellule, veuillez utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation). Lors du suivi des personnes à charge pour une cellule, toutes les formules du classeur ou de la feuille de calcul seront analysées et vérifiées.
C'est donc un processus chronophage. Si l'utilisateur a besoin de rechercher des personnes à charge pour de nombreuses cellules, l'utilisation de cette méthode
entraîner de mauvaises performances. Pour des raisons de performances, l'utilisateur doit utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation) à la place.
Ou, l'utilisateur peut d'abord rassembler la carte des précédents de toutes les cellules par [Cell.get_precedents()](/cells/fr/python-net/aspose.cells/cell/get_precedents),
puis construisez la carte des dépendances en fonction de la carte des précédents.

* Si une référence contenant cette cellule apparaît dans la formule d'une cellule, cette cellule sera considérée comme
la personne à charge de cette cellule, peu importe la référence ou cette cellule est utilisée ou non lors du calcul.
Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
cette formule est toujours considérée comme dépendante de A2.
Pour obtenir les formules dont les résultats calculés dépendent de cette cellule, veuillez utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation). Lors du suivi des personnes à charge pour une cellule, toutes les formules du classeur ou de la feuille de calcul seront analysées et vérifiées.
C'est donc un processus chronophage. Si l'utilisateur a besoin de rechercher des personnes à charge pour de nombreuses cellules, l'utilisation de cette méthode
entraîner de mauvaises performances. Pour des raisons de performances, l'utilisateur doit utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation) à la place.
Ou, l'utilisateur peut d'abord rassembler la carte des précédents de toutes les cellules par [Cell.get_precedents()](/cells/fr/python-net/aspose.cells/cell/get_precedents),
puis construisez la carte des dépendances en fonction de la carte des précédents.

* Si une référence contenant cette cellule apparaît dans la formule d'une cellule, cette cellule sera considérée comme
la personne à charge de cette cellule, peu importe la référence ou cette cellule est utilisée ou non lors du calcul.
Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul,
cette formule est toujours considérée comme dépendante de A2.
Pour obtenir les formules dont les résultats calculés dépendent de cette cellule, veuillez utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation). Lors du suivi des personnes à charge pour une cellule, toutes les formules du classeur ou de la feuille de calcul seront analysées et vérifiées.
C'est donc un processus chronophage. Si l'utilisateur a besoin de rechercher des personnes à charge pour de nombreuses cellules, l'utilisation de cette méthode
entraîner de mauvaises performances. Pour des raisons de performances, l'utilisateur doit utiliser [Cell.get_dependents_in_calculation(recursive)](/cells/fr/python-net/aspose.cells/cell/get_dependents_in_calculation) à la place.
Ou, l'utilisateur peut d'abord rassembler la carte des précédents de toutes les cellules par [Cell.get_precedents()](/cells/fr/python-net/aspose.cells/cell/get_precedents),
puis construisez la carte des dépendances en fonction de la carte des précédents.
###  Exemple

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
