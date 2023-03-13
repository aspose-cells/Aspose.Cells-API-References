---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | La cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field_name | str | Le nom de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | La cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field_index | int | L'index de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | La cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field | aspose.cells.pivot.PivotField | Le champ croisé dynamique dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
Ajouter un nouveau Slicer en utilisant ListObjet comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, table, index, dest_cell_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | Objet ListObject|
| index | int | L'index de ListColumn dans ListObject.ListColumns|
| dest_cell_name | str | La cellule dans le coin supérieur gauche de la plage Slicer.|

###  Exemple

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
Ajouter un nouveau Slicer en utilisant ListObjet comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | Objet ListObject|
| list_column | aspose.cells.tables.ListColumn | La ListColumn dans ListObject.ListColumns|
| dest_cell_name | str | La cellule dans le coin supérieur gauche de la plage Slicer.|

###  Exemple

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field_name | str | Le nom de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field_index | int | L'index de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Ajouter un nouveau Slicer en utilisant PivotTable comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| base_field | aspose.cells.pivot.PivotField | Le champ croisé dynamique dans PivotTable.BaseFields|

###  Exemple

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
Ajouter un nouveau Slicer en utilisant ListObjet comme source de données


###  Retour

Le nouvel index Slicer add


```python
def add(self, table, list_column, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | Objet ListObject|
| list_column | aspose.cells.tables.ListColumn | La ListColumn dans ListObject.ListColumns|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage Slicer.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage Slicer.|

###  Exemple

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



###  Voir également
* module [aspose.cells.slicers](../../)
* classe [SlicerCollection](/cells/fr/python-net/aspose.cells.slicers/slicercollection)
