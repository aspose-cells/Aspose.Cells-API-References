---
title: register_add_in_function méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 170
url: /fr/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Ajoute une fonction complémentaire dans le classeur


###  Retour

URL du fichier addin qui contient les fonctions addin


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| id | int | ID des données qui contiennent des fonctions complémentaires,<br/> peut être obtenu par le premier appel de [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/fr/python-net/aspose.cells/worksheetcollection/register_add_in_function) pour le même fichier addin.|
| function_name | str | le nom de la fonction complémentaire|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Ajoute une fonction complémentaire dans le classeur


###  Retour

ID des données contenant la fonction complémentaire donnée


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| add_in_file | str | le fichier contient les fonctions addin|
| function_name | str | le nom de la fonction complémentaire|
| lib | bool | si le fichier addin donné se trouve dans le répertoire ou le sous-répertoire de la bibliothèque Workbook Add-In.<br/>Cet indicateur prend effet et fait la différence lorsque addInFile est de chemin relatif :<br/> true indique que le chemin est relatif à la bibliothèque de compléments et false indique que le chemin est relatif à ce classeur.|



###  Voir également
* module [aspose.cells](../../)
* classe [WorksheetCollection](/cells/fr/python-net/aspose.cells/worksheetcollection)
