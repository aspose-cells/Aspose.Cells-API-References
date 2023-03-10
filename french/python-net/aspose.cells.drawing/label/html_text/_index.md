---
title: html_text propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 480
url: /fr/python-net/aspose.cells.drawing/label/html_text/
is_root: false
---
##  html_text propriété

Obtient et définit la chaîne html qui contient des données et certains formats dans cette zone de texte.

###  Exemple

```python

html = shape.html_text
if html == null  || html == "":
    shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Définition:
```python
@property
def html_text(self):
    ...
@html_text.setter
def html_text(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Label](/cells/fr/python-net/aspose.cells.drawing/label)
