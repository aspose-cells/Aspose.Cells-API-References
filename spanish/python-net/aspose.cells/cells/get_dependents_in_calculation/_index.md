---
title: get_dependents_in_calculation método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 390
url: /es/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Obtiene todas las celdas cuyo resultado calculado depende de una celda específica.


###  Devoluciones

Enumerador para enumerar todos los dependientes (objetos Cell)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| row | int | Índice de fila de la celda específica|
| column | int | Índice de columna de la celda específica.|
| recursive | bool | Si devuelve aquellos dependientes que no hacen referencia a la celda específica directamente<br/> sino referencia a otras hojas de esa celda.|
###  Observaciones

Para usar este método, asegúrese de que el libro de trabajo se haya configurado con el valor verdadero para
[FormulaSettings.enable_calculation_chain](/cells/es/python-net/aspose.cells/formulasettings#enable_calculation_chain) y se ha calculado completamente con esta configuración.
Si no hay una referencia de fórmula a esta celda, se devolverá un valor nulo.
Para obtener más detalles y ejemplos, consulte [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
