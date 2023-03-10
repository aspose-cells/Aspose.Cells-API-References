---
title: get_picture método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 120
url: /es/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Obtiene el objeto [Picture](/cells/es/python-net/aspose.cells.drawing/picture) del encabezado/pie de página.


###  Devoluciones

Devuelve el objeto [Picture](/cells/es/python-net/aspose.cells.drawing/picture).
Devuelve nulo si no hay imagen.


```python
def get_picture(self, is_header, section):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| is_header | bool | Indica si está en el encabezado o en el pie de página.|
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Obtiene el objeto [Picture](/cells/es/python-net/aspose.cells.drawing/picture) del encabezado/pie de página.


###  Devoluciones

Devuelve el objeto [Picture](/cells/es/python-net/aspose.cells.drawing/picture).


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| is_first | bool | Indica si se obtiene la imagen del encabezado/pie de página de la primera página.|
| is_even | bool | Indica si se obtiene la imagen del encabezado/pie de página par.|
| is_header | bool | Indica si se obtiene la imagen del encabezado/pie de página.|
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [PageSetup](/cells/es/python-net/aspose.cells/pagesetup)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
