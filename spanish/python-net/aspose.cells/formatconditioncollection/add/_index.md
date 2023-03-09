---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/formatconditioncollection/add/
is_root: false
---
##  add(cell_area, type, operator_type, formula1, formula2) {#CellArea-FormatConditionType-OperatorType-str-str}
Agrega una condición de formato y un rango de celda afectado a FormatConditions
FormatConditions puede contener hasta tres formatos condicionales.
Las referencias a las otras hojas no están permitidas en las fórmulas de formato condicional.


###  Devoluciones

[0]: Índice de objeto de condición de formato; [1] Índice de rango de celda afectado.


```python
def add(self, cell_area, type, operator_type, formula1, formula2):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell_area | [CellArea](/cells/es/python-net/aspose.cells/cellarea) |Rango de celdas con formato condicional.|
| type | [FormatConditionType](/cells/es/python-net/aspose.cells/formatconditiontype) | Tipo de formato condicional. Podría ser uno de los miembros de FormatConditionType.|
| operator_type | [OperatorType](/cells/es/python-net/aspose.cells/operatortype) | Operador de comparación Podría ser uno de los miembros de OperatorType.|
| formula1 | str | El valor o la expresión asociada con el formato condicional.|
| formula2 | str | El valor o la expresión asociada con el formato condicional|



###  Ver también
* módulo [aspose.cells](../../)
* clase [FormatConditionCollection](/cells/es/python-net/aspose.cells/formatconditioncollection)
