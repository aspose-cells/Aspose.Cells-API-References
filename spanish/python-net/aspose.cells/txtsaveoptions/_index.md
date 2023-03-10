---
title: TxtSaveOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1520
url: /es/python-net/aspose.cells/txtsaveoptions/
is_root: false
---
##  TxtSaveOptions clase
Representa las opciones de guardado para csv/delimitado por tabuladores/otro formato de texto.



**Herencia:** [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions) → 
[SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)



El tipo TxtSaveOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [TxtSaveOptions()](/cells/es/python-net/aspose.cells/txtsaveoptions/__init__/#) | Crea opciones para guardar archivos de texto.|
| [TxtSaveOptions(format)](/cells/es/python-net/aspose.cells/txtsaveoptions/__init__/#SaveFormat) | Crea opciones para guardar archivos de texto.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells/txtsaveoptions/save_format) | Obtiene el formato de archivo guardado.|
| [clear_data](/cells/es/python-net/aspose.cells/txtsaveoptions/clear_data) | Vacíe el libro de trabajo después de guardar el archivo.|
| [cached_file_folder](/cells/es/python-net/aspose.cells/txtsaveoptions/cached_file_folder) | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño.|
| [validate_merged_areas](/cells/es/python-net/aspose.cells/txtsaveoptions/validate_merged_areas) | Indica si validar las celdas combinadas antes de guardar el archivo.|
| [merge_areas](/cells/es/python-net/aspose.cells/txtsaveoptions/merge_areas) | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo.|
| [create_directory](/cells/es/python-net/aspose.cells/txtsaveoptions/create_directory) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.|
| [sort_names](/cells/es/python-net/aspose.cells/txtsaveoptions/sort_names) | Indica si ordenar los nombres definidos antes de guardar el archivo.|
| [sort_external_names](/cells/es/python-net/aspose.cells/txtsaveoptions/sort_external_names) |Indica si ordenar los nombres definidos externos antes de guardar el archivo.|
| [refresh_chart_cache](/cells/es/python-net/aspose.cells/txtsaveoptions/refresh_chart_cache) | Indica si se actualizan los datos de la memoria caché del gráfico|
| [warning_callback](/cells/es/python-net/aspose.cells/txtsaveoptions/warning_callback) | Obtiene o establece una devolución de llamada de advertencia.|
| [update_smart_art](/cells/es/python-net/aspose.cells/txtsaveoptions/update_smart_art) | Indica si se está actualizando la configuración de arte inteligente.<br/> El valor predeterminado es falso.|
| [separator](/cells/es/python-net/aspose.cells/txtsaveoptions/separator) | Obtiene y establece el delimitador de caracteres del archivo de texto.|
| [separator_string](/cells/es/python-net/aspose.cells/txtsaveoptions/separator_string) | Obtiene y establece un valor de cadena como separador.|
| [encoding](/cells/es/python-net/aspose.cells/txtsaveoptions/encoding) | Obtiene y establece la codificación predeterminada.|
| [always_quoted](/cells/es/python-net/aspose.cells/txtsaveoptions/always_quoted) | Indica si siempre se añade '"' para cada campo.<br/>Si es verdadero, se citarán todos los valores;<br/>Si es falso, los valores solo se citarán cuando sea necesario (por ejemplo,<br/>cuando los valores contienen caracteres especiales como '"' , '\n' o carácter separador).<br/> El valor predeterminado es falso.|
| [quote_type](/cells/es/python-net/aspose.cells/txtsaveoptions/quote_type) | Obtiene o establece cómo citar valores en el archivo de texto exportado.|
| [format_strategy](/cells/es/python-net/aspose.cells/txtsaveoptions/format_strategy) | Obtiene y establece la estrategia de formato al exportar el valor de la celda como una cadena.|
| [light_cells_data_provider](/cells/es/python-net/aspose.cells/txtsaveoptions/light_cells_data_provider) | El proveedor de datos para proporcionar datos de celdas para guardar el libro de trabajo en modo ligero.|
| [trim_leading_blank_row_and_column](/cells/es/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column) | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace MS Excel.<br/> El valor predeterminado es verdadero.|
| [trim_tailing_blank_cells](/cells/es/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells) | Indica si se deben recortar las celdas en blanco de cola en una fila. El valor predeterminado es falso.|
| [keep_separators_for_blank_row](/cells/es/python-net/aspose.cells/txtsaveoptions/keep_separators_for_blank_row) | Indica si se deben generar separadores para filas en blanco.<br/> El valor predeterminado es falso, por lo que el contenido de la fila en blanco estará vacío de forma predeterminada.|
| [export_area](/cells/es/python-net/aspose.cells/txtsaveoptions/export_area) | El rango de celdas a exportar.|
| [export_quote_prefix](/cells/es/python-net/aspose.cells/txtsaveoptions/export_quote_prefix) | Indica si el signo de comillas simples debe exportarse como parte del valor de una celda<br/> cuando [Style.quote_prefix](/cells/es/python-net/aspose.cells/style#quote_prefix) es cierto para ello. El valor predeterminado es falso.|
| [export_all_sheets](/cells/es/python-net/aspose.cells/txtsaveoptions/export_all_sheets) |Indica si exportar todas las hojas al archivo de texto.<br/> Si es falso, solo exporte la hoja activa, al igual que MS Excel.|



###  Ver también
* módulo [aspose.cells](..)
* clase [SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)
* clase [TxtSaveOptions](/cells/es/python-net/aspose.cells/txtsaveoptions)
