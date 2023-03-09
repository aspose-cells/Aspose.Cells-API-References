---
title: AbstractCalculationMonitor clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor clase
Monitor para que el usuario siga el progreso del cálculo de la fórmula.



El tipo AbstractCalculationMonitor expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [original_value](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Obtiene el valor antiguo de la celda calculada.<br/> Debe usarse solo en [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) y [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Si el valor de la celda ha cambiado después del cálculo.<br/> Debe usarse solo en [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Obtiene el valor recién calculado de la celda.<br/> Debe usarse solo en [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  Métodos
| Método| Descripción|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Implemente este método para hacer negocios antes de calcular una celda.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Implemente este método para hacer negocios después de que se haya calculado una celda.|
| [on_circular(circular_cells_data)](/cells/es/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Implemente este método para hacer negocios al calcular fórmulas con referencias circulares.|



###  Ver también
* módulo [aspose.cells](..)
