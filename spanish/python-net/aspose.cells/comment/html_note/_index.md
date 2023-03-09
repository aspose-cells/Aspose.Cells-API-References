---
title: html_note propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 140
url: /es/python-net/aspose.cells/comment/html_note/
is_root: false
---
##  html_note propiedad

Obtiene y establece la cadena html que contiene datos y algunos formatos en este comentario.

###  Observaciones

Si se trata de un comentario encadenado, la nota no se puede cambiar; de lo contrario, MS Excel no podría procesarlo como un comentario encadenado.

###  Ejemplo

```python

comment1.html_note = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Definición:
```python
@property
def html_note(self):
    ...
@html_note.setter
def html_note(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Comment](/cells/es/python-net/aspose.cells/comment)
