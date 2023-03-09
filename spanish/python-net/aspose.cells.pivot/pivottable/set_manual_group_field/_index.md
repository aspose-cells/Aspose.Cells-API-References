---
title: set_manual_group_field método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 210
url: /es/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/
is_root: false
---
##  set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-float-float-list-float}
Establece el grupo de campos manual por la tabla dinámica.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| base_field_index | int | El índice de campo de fila o columna en los campos base|
| start_val | float |Especifica el valor inicial para la agrupación numérica.|
| end_val | float | Especifica el valor final para la agrupación numérica.|
| group_by_list | list | Especifica la lista de tipos de agrupación. Especificado por PivotTableGroupType|
| interval_num | float | Especifica el grupo de números de intervalo por agrupación numérica.|


##  set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-float-float-list-float}
Establece el grupo de campos manual por la tabla dinámica.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| pivot_field | [PivotField](/cells/es/python-net/aspose.cells.pivot/pivotfield) | El campo de fila o columna en los campos base|
| start_val | float |Especifica el valor inicial para la agrupación numérica.|
| end_val | float | Especifica el valor final para la agrupación numérica.|
| group_by_list | list | Especifica la lista de tipos de agrupación. Especificado por PivotTableGroupType|
| interval_num | float | Especifica el grupo de números de intervalo por agrupación numérica.|


##  set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-DateTime-DateTime-list-int}
Establece el grupo de campos manual por la tabla dinámica.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| base_field_index | int | El índice de campo de fila o columna en los campos base|
| start_val | DateTime | Especifica el valor inicial para la agrupación de fechas.|
| end_val | DateTime | Especifica el valor final para la agrupación de fechas.|
| group_by_list | list | Especifica la lista de tipos de agrupación. Especificado por PivotTableGroupType|
| interval_num | int | Especifica el grupo de números de intervalo por agrupación de días. El número de días debe ser un entero positivo distinto de cero|


##  set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-DateTime-DateTime-list-int}
Establece el grupo de campos manual por la tabla dinámica.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| pivot_field | [PivotField](/cells/es/python-net/aspose.cells.pivot/pivotfield) | El campo de fila o columna en los campos base|
| start_val | DateTime | Especifica el valor inicial para la agrupación de fechas.|
| end_val | DateTime | Especifica el valor final para la agrupación de fechas.|
| group_by_list | list | Especifica la lista de tipos de agrupación. Especificado por PivotTableGroupType|
| interval_num | int | Especifica el grupo de números de intervalo por agrupación de días. El número de días debe ser un entero positivo distinto de cero|



###  Ver también
* módulo [aspose.cells.pivot](../../)
* clase [PivotTable](/cells/es/python-net/aspose.cells.pivot/pivottable)
