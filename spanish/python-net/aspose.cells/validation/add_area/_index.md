---
title: add_area método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Aplica la validación al área.



```python
def add_area(self, cell_area):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell_area | [CellArea](/cells/es/python-net/aspose.cells/cellarea) | La zona.|
###  Observaciones

Es equivalente a usar [Validation.add_area(cell_area)](/cells/es/python-net/aspose.cells/validation/add_area)
con comprobación de intersecciones y bordes.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Aplica la validación al área.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell_area | [CellArea](/cells/es/python-net/aspose.cells/cellarea) | La zona.|
| check_intersection | bool | Si verifica la intersección del área dada con las áreas de validaciones existentes.<br/>Si se ha aplicado una validación en un área determinada (o parte de ella),<br/>entonces la validación existente debe eliminarse al principio del área dada.<br/>De lo contrario, las Validaciones generadas pueden causar corrupción.<br/>Si el usuario está seguro de que el área agregada no se cruza con ningún área existente,<br/> Este parámetro se puede establecer como falso para tener en cuenta el rendimiento.|
| check_edge | bool | Si comprueba el borde de las áreas aplicadas de esta validación.<br/>La configuración interna de la validación depende del rango superior izquierdo de sus rangos aplicados,<br/>entonces, si el área dada se convertirá en la nueva parte superior izquierda de los rangos aplicados,<br/>la configuración interna debe cambiarse y reconstruirse; de lo contrario, se pueden producir resultados inesperados.<br/>Si el usuario está seguro de que el área agregada no es la de arriba a la izquierda,<br/> Este parámetro se puede establecer como falso para tener en cuenta el rendimiento.|
###  Observaciones

En este método, eliminaremos todas las validaciones antiguas en un área determinada.
Para el rango superior izquierdo de los rangos aplicados de Validación, en primer lugar, su StartRow es el más pequeño,
en segundo lugar, su StartColumn es la más pequeña de esas áreas que tienen el mismo StartRow más pequeño.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Validation](/cells/es/python-net/aspose.cells/validation)
