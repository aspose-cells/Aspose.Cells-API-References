---
title: get_leafs método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 160
url: /es/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Obtenga todas las celdas que hacen referencia a esta celda directamente y deben actualizarse cuando se modifica esta celda.


###  Devoluciones

Enumerador para enumerar todos los dependientes (Cell)


```python
def get_leafs(self):
    ...
```


###  Observaciones

NOTA: Esta clase ahora está obsoleta. En cambio,
utilice Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo.
Esta propiedad se eliminará 12 meses después desde mayo de 2022.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

##  get_leafs(recursive) {#bool}
Obtenga todas las celdas que se actualizarán cuando se modifique esta celda.


###  Devoluciones

Enumerador para enumerar todos los dependientes (Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| recursive | bool | Si devuelve aquellas hojas que no hacen referencia a esta celda directamente<br/> pero referencia a otras hojas de esta celda|
###  Observaciones

NOTA: Esta clase ahora está obsoleta. En cambio,
utilice Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo.
Esta propiedad se eliminará 12 meses después desde mayo de 2022.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
