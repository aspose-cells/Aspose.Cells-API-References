---
title: get_linked_cell método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells.drawing/webextensionshape/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Obtiene el rango vinculado al valor del control.


###  Devoluciones

El rango vinculado al valor del control.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| is_r1c1 | bool | Si la fórmula debe formatearse como R1C1.|
| is_local | bool | Si la fórmula debe formatearse según la configuración regional.|

###  Ejemplos

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [WebExtensionShape](/cells/es/python-net/aspose.cells.drawing/webextensionshape)
