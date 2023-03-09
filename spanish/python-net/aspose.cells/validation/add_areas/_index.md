---
title: add_areas método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/validation/add_areas/
is_root: false
---
##  add_areas(areas, check_intersection, check_edge) {#list-bool-bool}
Aplica la validación a áreas dadas.



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| areas | list | Las areas.|
| check_intersection | bool | Si verifica la intersección del área dada con las áreas de validaciones existentes.<br/>Si se ha aplicado una validación en un área determinada (o parte de ella),<br/>entonces la validación existente debe eliminarse al principio del área dada.<br/>De lo contrario, se pueden producir daños en las Validaciones generadas.<br/>Si el usuario está seguro de que todas las áreas agregadas no se cruzan con ninguna área existente,<br/> este parámetro se puede establecer como falso para considerar el rendimiento.|
| check_edge | bool | Si comprueba el borde de las áreas aplicadas de esta validación.<br/>La configuración interna de la validación depende del rango superior izquierdo de sus rangos aplicados,<br/>entonces, si una de las áreas dadas se convertirá en la nueva superior izquierda de los rangos aplicados,<br/>la configuración interna debe cambiarse y reconstruirse; de lo contrario, se pueden producir resultados inesperados.<br/>Si el usuario está seguro de que ninguna de esas áreas agregadas es la parte superior izquierda,<br/> este parámetro se puede establecer como falso para considerar el rendimiento.|
###  Observaciones

En este método, eliminaremos todas las validaciones antiguas en un área determinada.
Para el rango superior izquierdo de los rangos aplicados de Validación, en primer lugar, su StartRow es el más pequeño,
en segundo lugar, su StartColumn es la más pequeña de esas áreas que tienen el mismo StartRow más pequeño.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Validation](/cells/es/python-net/aspose.cells/validation)
