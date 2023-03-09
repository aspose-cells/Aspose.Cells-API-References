---
title: WorkbookDesigner clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1600
url: /es/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner clase
Encapsula el objeto que representa una hoja de cálculo de diseñador.



El tipo WorkbookDesigner expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [WorkbookDesigner()](/cells/es/python-net/aspose.cells/workbookdesigner/__init__/#) | Inicializa una nueva instancia de la clase [WorkbookDesigner](/cells/es/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/es/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Inicializa una nueva instancia de la clase [WorkbookDesigner](/cells/es/python-net/aspose.cells/workbookdesigner).|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [workbook](/cells/es/python-net/aspose.cells/workbookdesigner/workbook) | Obtiene y establece el objeto [WorkbookDesigner.workbook](/cells/es/python-net/aspose.cells/workbookdesigner#workbook).|
| [repeat_formulas_with_subtotal](/cells/es/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Indica si se repiten fórmulas con fila de subtotal.|
| [update_empty_string_as_null](/cells/es/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | Si es VERDADERO, se insertará Nulo si el valor es "";|
| [update_reference](/cells/es/python-net/aspose.cells/workbookdesigner/update_reference) | Indica si se actualizarán las referencias en otras hojas de trabajo.|
| [calculate_formula](/cells/es/python-net/aspose.cells/workbookdesigner/calculate_formula) | Indica si se deben calcular las fórmulas.|
| [call_back](/cells/es/python-net/aspose.cells/workbookdesigner/call_back) | Obtiene y establece la interfaz de devolución de llamada de procesamiento de marcador inteligente.|
| [line_by_line](/cells/es/python-net/aspose.cells/workbookdesigner/line_by_line) | Indica si se está procesando el marcador inteligente línea por línea.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/es/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Establece la fuente de datos de un objeto [ICellsDataTable](/cells/es/python-net/aspose.cells/icellsdatatable).|
| [set_data_source(variable, data)](/cells/es/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Establece el enlace de datos a una variable.|
| [process()](/cells/es/python-net/aspose.cells/workbookdesigner/process/#) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.|
| [process(is_preserved)](/cells/es/python-net/aspose.cells/workbookdesigner/process/#bool) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.|
| [process(sheet_index, is_preserved)](/cells/es/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.|
| [clear_data_source()](/cells/es/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Borra todas las fuentes de datos.|
| [get_smart_markers()](/cells/es/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Devuelve una colección de marcadores inteligentes en una hoja de cálculo.|



###  Ejemplo

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [ICellsDataTable](/cells/es/python-net/aspose.cells/icellsdatatable)
* clase [WorkbookDesigner](/cells/es/python-net/aspose.cells/workbookdesigner)
