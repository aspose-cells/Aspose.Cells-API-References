---
title: clear método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Elimina todos los enlaces externos.



```python
def clear(self):
    ...
```


###  Observaciones

Al eliminar enlaces externos, todas las fórmulas que hacen referencia a ellos también se eliminarán porque
las referencias dejan de ser válidas.

##  clear(update_references_as_local) {#bool}
Elimina todos los enlaces externos.



```python
def clear(self, update_references_as_local):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| update_references_as_local | bool | Si actualiza todas las referencias de enlaces externos como referencias del propio libro de trabajo actual.|
###  Observaciones

Si es necesario actualizar las referencias, las referencias a enlaces externos en fórmulas se cambiarán al libro de trabajo actual.
Por ejemplo, la fórmula original de una celda es "='fuenteexterna.xlam'!funciónpersonalizada()",
después de eliminar los enlaces externos, la fórmula se convertirá en "=función personalizada()".
Si no es necesario actualizar las referencias, todas las fórmulas con referencias a enlaces externos
también se eliminará porque esas referencias dejan de ser válidas.


###  Ver también
* módulo [aspose.cells](../../)
* clase [ExternalLinkCollection](/cells/es/python-net/aspose.cells/externallinkcollection)
