---
title: remove_at método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Elimina el vínculo externo especificado del libro de trabajo.



```python
def remove_at(self, index):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| index | int | el índice del enlace externo que se va a eliminar.|
###  Observaciones

Al eliminar el enlace externo, todas las fórmulas que hacen referencia a él también se eliminarán porque
las referencias dejan de ser válidas.

##  remove_at(index, update_references_as_local) {#int-bool}
Elimina el vínculo externo especificado del libro de trabajo.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| index | int | el índice del enlace externo que se va a eliminar.|
| update_references_as_local | bool | Si actualiza todas las referencias del enlace externo dado a la referencia del libro de trabajo actual.|
###  Observaciones

Si es necesario actualizar las referencias, las referencias a enlaces externos en fórmulas se cambiarán al libro de trabajo actual.
Por ejemplo, el enlace externo que se eliminará es "externalsource.xlam" y define una función personalizada "función personalizada()",
la fórmula original de una celda es "='fuenteexterna.xlam'!funciónpersonalizada()",
después de eliminar la fórmula se convertirá en "=función personalizada()".
Si no es necesario actualizar la referencia, todas las fórmulas con referencia a este enlace externo
también se eliminará porque esas referencias dejan de ser válidas.


###  Ver también
* módulo [aspose.cells](../../)
* clase [ExternalLinkCollection](/cells/es/python-net/aspose.cells/externallinkcollection)
