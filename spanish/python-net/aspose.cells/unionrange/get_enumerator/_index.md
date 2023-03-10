---
title: get_enumerator método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/unionrange/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Obtiene el enumerador de las celdas de este rango.


###  Devoluciones

El enumerador de células


```python
def get_enumerator(self):
    ...
```


###  Observaciones

Al atravesar elementos por el Enumerador devuelto, la colección de celdas
no debe modificarse (como las operaciones que harán que se cree una nueva fila Cell o que se elimine la fila Cell existente).
De lo contrario, es posible que el enumerador no pueda recorrer todas las celdas correctamente (algunos elementos pueden recorrerse repetidamente u omitirse).


###  Ver también
* módulo [aspose.cells](../../)
* clase [UnionRange](/cells/es/python-net/aspose.cells/unionrange)
