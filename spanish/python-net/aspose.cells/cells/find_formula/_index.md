---
title: find_formula método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 300
url: /es/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
Encuentra la celda con la cadena de entrada.


###  Devoluciones

Cell objeto.


```python
def find_formula(self, formula, previous_cell):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| formula | str | La fórmula a buscar.|
| previous_cell | [Cell](/cells/es/python-net/aspose.cells/cell) |Celda anterior con la misma fórmula. Este parámetro se puede establecer en nulo si se busca desde el principio.|
###  Observaciones

Devuelve nulo (nada) si no se encuentra ninguna celda.
 NOTA: Este miembro ahora está obsoleto.
utilice el método Cells.Find(object,Cell,FindOptions) con LookInType como LookInType.OnlyFormulas
 y LookAtType como LookAtType.EntireContent.
 Este miembro será eliminado 12 meses después desde noviembre de 2018.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
