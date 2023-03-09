---
title: ExportTableOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 550
url: /es/python-net/aspose.cells/exporttableoptions/
is_root: false
---
##  ExportTableOptions clase
Representa todas las opciones de tabla de exportación.



El tipo ExportTableOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [ExportTableOptions()](/cells/es/python-net/aspose.cells/exporttableoptions/__init__/#) | Construye una nueva instancia de ExportTableOptions|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [export_column_name](/cells/es/python-net/aspose.cells/exporttableoptions/export_column_name) | Indica si los datos de la primera fila se exportan al nombre de columna de DataTable.<br/> El valor predeterminado es falso.|
| [skip_error_value](/cells/es/python-net/aspose.cells/exporttableoptions/skip_error_value) | Indica si se salta un valor no válido para la columna.<br/> Por ejemplo, si el tipo de columna es decimal, el valor es mayor que decimal.MaxValue<br/>y esta propiedad es verdadera, no volveremos a lanzar una excepción.<br/> El valor predeterminado es falso.|
| [plot_visible_cells](/cells/es/python-net/aspose.cells/exporttableoptions/plot_visible_cells) | Solo exporta celdas visibles.|
| [plot_visible_rows](/cells/es/python-net/aspose.cells/exporttableoptions/plot_visible_rows) | Solo exporta filas visibles.|
| [plot_visible_columns](/cells/es/python-net/aspose.cells/exporttableoptions/plot_visible_columns) | Solo exporta columnas visibles.|
| [export_as_string](/cells/es/python-net/aspose.cells/exporttableoptions/export_as_string) | Exporta el valor de cadena de las celdas a DataTable.|
| [export_as_html_string](/cells/es/python-net/aspose.cells/exporttableoptions/export_as_html_string) | Exporta el valor de cadena html de las celdas a DataTable.|
| [format_strategy](/cells/es/python-net/aspose.cells/exporttableoptions/format_strategy) | Obtiene y establece la estrategia de formato al exportar el valor como valor de cadena.|
| [check_mixed_value_type](/cells/es/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) |Falso, Aspose.Cells establecerá el tipo de DataColumn según el tipo de valor de la primera fila para el rendimiento.<br/> Cierto, Aspose.Cells verificará si el tipo de valor en la columna se mezcla antes de establecer el tipo de DataColumn<br/> Y el tipo de valor se mezcla, el tipo de DataColumn será una cadena.|
| [is_vertical](/cells/es/python-net/aspose.cells/exporttableoptions/is_vertical) | True si una fila en el archivo Workbook representa una fila en DataTable. Falso si una columna en el archivo Workbook representa una fila en DataTable.|
| [indexes](/cells/es/python-net/aspose.cells/exporttableoptions/indexes) |Los índices de columnas/filas que deben exportarse.|
| [rename_strategy](/cells/es/python-net/aspose.cells/exporttableoptions/rename_strategy) | Estrategia para nombres duplicados de columnas.|



###  Ver también
* módulo [aspose.cells](..)
