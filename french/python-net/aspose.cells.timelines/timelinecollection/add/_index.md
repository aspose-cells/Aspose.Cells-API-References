---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field_name | str | Le nom de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field_index | int | L'index de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| dest_cell_name | str | Le nom de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field | aspose.cells.pivot.PivotField | Le champ croisé dynamique dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field_name | str | Le nom de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field_index | int | L'index de PivotField dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données


###  Retour

Le nouvel index de la chronologie add


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objet tableau croisé dynamique|
| row | int | Index de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| column | int | Index de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie.|
| base_field | aspose.cells.pivot.PivotField | Le champ croisé dynamique dans PivotTable.BaseFields|

###  Exemple

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  Voir également
* module [aspose.cells.timelines](../../)
* classe [TimelineCollection](/cells/fr/python-net/aspose.cells.timelines/timelinecollection)
