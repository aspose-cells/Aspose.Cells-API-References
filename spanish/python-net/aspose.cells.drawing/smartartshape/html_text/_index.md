---
title: html_text propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 480
url: /es/python-net/aspose.cells.drawing/smartartshape/html_text/
is_root: false
---
##  html_text propiedad

Obtiene y establece la cadena html que contiene datos y algunos formatos en este cuadro de texto.

###  Ejemplo

```python

html = shape.html_text
if html == null  || html == "":
    shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Definición:
```python
@property
def html_text(self):
    ...
@html_text.setter
def html_text(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [SmartArtShape](/cells/es/python-net/aspose.cells.drawing/smartartshape)
