---
title: import_custom_objects méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 640
url: /fr/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
Importe des objets personnalisés.


###  Retour

Nombre total de lignes importées.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| list | list | L'objet personnalisé|
| first_row | int | Le numéro de ligne de la première cellule à importer.|
| first_column | int | Le numéro de colonne de la première cellule à importer.|
| options | [ImportTableOptions](/cells/fr/python-net/aspose.cells/importtableoptions) | Les options d'importation.|
###  Remarques

Les objets personnalisés doivent être du même type.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

Importe des objets personnalisés.


###  Retour

Nombre total de lignes importées.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| list | list | L'objet personnalisé|
| property_names | list | Les noms de propriété. S'il est nul, nous importerons toutes les propriétés de l'objet.|
| is_property_name_shown | bool | Indique si le nom de la propriété sera importé dans la première ligne.|
| first_row | int | Le numéro de ligne de la première cellule à importer.|
| first_column | int | Le numéro de colonne de la première cellule à importer.|
| row_number | int | Nombre de lignes à importer.|
| insert_rows | bool | Indique si des lignes supplémentaires sont ajoutées pour ajuster les données.|
| date_format_string | str | Chaîne de format de date pour les cellules.|
| convert_string_to_number | bool | Indique si cette méthode tentera de convertir une chaîne en nombre.|
###  Remarques

Les objets personnalisés doivent être du même type.


###  Voir également

* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
