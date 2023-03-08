---
title: html_text Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 480
url: /de/python-net/aspose.cells.drawing/cellsdrawing/html_text/
is_root: false
---
##  html_text Eigentum

Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formate in diesem Textfeld enthält.

###  Beispiel

```python

html = shape.html_text
if html == null  || html == "":
    shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Definition:
```python
@property
def html_text(self):
    ...
@html_text.setter
def html_text(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [CellsDrawing](/cells/de/python-net/aspose.cells.drawing/cellsdrawing)
