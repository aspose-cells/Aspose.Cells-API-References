---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.


###  Retour

[Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink) indice d'objet.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell_name | str | Cell nom.|
| total_rows | int | Nombre de lignes dans cette plage de liens hypertexte.|
| total_columns | int | Nombre de colonnes de cette plage de liens hypertexte.|
| address | str | Adresse du lien hypertexte.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.


###  Retour

[Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink) indice d'objet.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| first_row | int | Première ligne de la plage de liens hypertexte.|
| first_column | int | Première colonne de la plage de liens hypertexte.|
| total_rows | int | Nombre de lignes dans cette plage de liens hypertexte.|
| total_columns | int | Nombre de colonnes de cette plage de liens hypertexte.|
| address | str | Adresse du lien hypertexte.|

###  Exemples

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.


###  Retour

[Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink) indice d'objet.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| start_cell_name | str | La cellule supérieure gauche de la plage.|
| end_cell_name | str | La cellule en bas à droite de la plage.|
| address | str | Adresse du lien hypertexte.|
| text_to_display | str | Texte à afficher pour le lien hypertexte spécifié.|
| screen_tip | str |Le texte de l'info-bulle pour le lien hypertexte spécifié.|



###  Voir également
* module [aspose.cells](../../)
* classe [Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink)
* classe [HyperlinkCollection](/cells/fr/python-net/aspose.cells/hyperlinkcollection)
