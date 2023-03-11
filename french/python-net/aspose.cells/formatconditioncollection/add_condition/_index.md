---
title: add_condition méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
Ajoutez une condition de mise en forme.


###  Retour

Index d'objet de condition de formatage ;


```python
def add_condition(self, type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [FormatConditionType](/cells/fr/python-net/aspose.cells/formatconditiontype) | Formater le type de condition.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
Ajoute une condition de formatage.


###  Retour

Index d'objet de condition de formatage ;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [FormatConditionType](/cells/fr/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/fr/python-net/aspose.cells/formatconditiontype) de mise en forme conditionnelle.<br/> Il peut s'agir de l'un des membres de FormatConditionType.|
| operator_type | [OperatorType](/cells/fr/python-net/aspose.cells/operatortype) | La comparaison [OperatorType](/cells/fr/python-net/aspose.cells/operatortype).<br/> Il peut s'agir de l'un des membres de OperatorType.|
| formula1 | str | La valeur ou l'expression associée à la mise en forme conditionnelle.<br/>Si la valeur d'entrée commence par '=', elle sera considérée comme une formule.<br/>Sinon, il sera pris comme valeur simple (texte, nombre, booléen).<br/> Pour une valeur de texte commençant par '=', l'utilisateur peut la saisir sous forme de formule au format : "=\"=...\"".|
| formula2 | str | La valeur ou l'expression associée à la mise en forme conditionnelle.<br/>Le format d'entrée est le même avec formula1|



###  Voir également
* module [aspose.cells](../../)
* classe [FormatConditionCollection](/cells/fr/python-net/aspose.cells/formatconditioncollection)
* classe [FormatConditionType](/cells/fr/python-net/aspose.cells/formatconditiontype)
* classe [OperatorType](/cells/fr/python-net/aspose.cells/operatortype)
