---
title: get_style método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/row/get_style/
is_root: false
---
##  get_style() {#}
Obtiene el estilo de esta fila.



```python
def get_style(self):
    ...
```


###  Observaciones

La modificación directa del objeto de estilo devuelto no tiene efecto para esta fila ni para ninguna de las celdas de esta fila.
Tienes que llamar al [Row.apply_style(style, flag)](/cells/es/python-net/aspose.cells/row/apply_style) o al método [Row.set_style(style)](/cells/es/python-net/aspose.cells/row/set_style)
para aplicar el cambio a esta fila.

El estilo de la fila es el estilo que heredarán las celdas de esta fila (las celdas que no tienen una configuración de estilo personalizada,
como celdas existentes a las que no se les ha establecido un estilo de forma explícita, o aquellas que no han sido instanciadas)


###  Ver también
* módulo [aspose.cells](../../)
* clase [Row](/cells/es/python-net/aspose.cells/row)
