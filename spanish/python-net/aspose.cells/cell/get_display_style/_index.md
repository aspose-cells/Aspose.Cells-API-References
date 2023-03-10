---
title: get_display_style método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 110
url: /es/python-net/aspose.cells/cell/get_display_style/
is_root: false
---
##  get_display_style() {#}
Obtiene el estilo de visualización de la celda.
Si esta celda también se ve afectada por otras configuraciones, como el formato condicional, la lista de objetos, etc.,
entonces el estilo de visualización puede ser diferente de cell.GetStyle().



```python
def get_display_style(self):
    ...
```




##  get_display_style(include_merged_borders) {#bool}
Obtiene el estilo de visualización de la celda.
Si la celda tiene formato condicional, el estilo de visualización no es el mismo que el de cell.GetStyle().



```python
def get_display_style(self, include_merged_borders):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| include_merged_borders | bool | Indica si se revisan los bordes de las celdas combinadas.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
