---
title: OdsLoadOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1100
url: /es/python-net/aspose.cells/odsloadoptions/
is_root: false
---
##  OdsLoadOptions clase
Representa las opciones de carga del archivo ods.



**Herencia:** [OdsLoadOptions](/cells/python-net/aspose.cells/odsloadoptions) → 
[LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)



El tipo OdsLoadOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [OdsLoadOptions()](/cells/es/python-net/aspose.cells/odsloadoptions/__init__/#) | Representa las opciones de carga del archivo ods.|
| [OdsLoadOptions(type)](/cells/es/python-net/aspose.cells/odsloadoptions/__init__/#LoadFormat) | Representa las opciones de carga del archivo ods.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [load_format](/cells/es/python-net/aspose.cells/odsloadoptions/load_format) | Obtiene el formato de carga.|
| [password](/cells/es/python-net/aspose.cells/odsloadoptions/password) | Obtiene y establece la contraseña del libro de trabajo.|
| [parsing_formula_on_open](/cells/es/python-net/aspose.cells/odsloadoptions/parsing_formula_on_open) | Indica si se analiza la fórmula al leer el archivo.|
| [parsing_pivot_cached_records](/cells/es/python-net/aspose.cells/odsloadoptions/parsing_pivot_cached_records) | Indica si se están analizando los registros en caché dinámicos al cargar el archivo.<br/> El valor predeterminado es falso.|
| [language_code](/cells/es/python-net/aspose.cells/odsloadoptions/language_code) | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo en función del código de país que guardó el archivo.|
| [region](/cells/es/python-net/aspose.cells/odsloadoptions/region) | Obtiene o establece la configuración regional del sistema según el código de país en el momento en que se cargó el archivo.|
| [default_style_settings](/cells/es/python-net/aspose.cells/odsloadoptions/default_style_settings) | Obtiene la configuración de estilo predeterminada para inicializar estilos del libro de trabajo|
| [standard_font](/cells/es/python-net/aspose.cells/odsloadoptions/standard_font) | Establece el nombre de fuente estándar predeterminado|
| [standard_font_size](/cells/es/python-net/aspose.cells/odsloadoptions/standard_font_size) | Establece el tamaño de fuente estándar predeterminado.|
| [interrupt_monitor](/cells/es/python-net/aspose.cells/odsloadoptions/interrupt_monitor) | Obtiene y establece el monitor de interrupciones.|
| [ignore_not_printed](/cells/es/python-net/aspose.cells/odsloadoptions/ignore_not_printed) | Ignore los datos que no se imprimen si imprime directamente el archivo|
| [check_data_valid](/cells/es/python-net/aspose.cells/odsloadoptions/check_data_valid) |Compruebe si los datos son válidos en el archivo de plantilla.|
| [check_excel_restriction](/cells/es/python-net/aspose.cells/odsloadoptions/check_excel_restriction) | Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas.<br/>Por ejemplo, Excel no permite ingresar un valor de cadena de más de 32K.<br/>Cuando ingresa un valor de más de 32 K, como Cell.PutValue (cadena), si esta propiedad es verdadera, obtendrá una excepción.<br/>Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego<br/>puede generar el valor de cadena completo para otros formatos de archivo como CSV.<br/>Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel,<br/> no debe guardar el libro de trabajo como formato de archivo de Excel más adelante. De lo contrario, puede haber un error inesperado para el archivo de Excel generado.|
| [keep_unparsed_data](/cells/es/python-net/aspose.cells/odsloadoptions/keep_unparsed_data) | Si mantiene los datos no analizados en la memoria para el libro de trabajo cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.|
| [load_filter](/cells/es/python-net/aspose.cells/odsloadoptions/load_filter) | El filtro para indicar cómo cargar datos.|
| [light_cells_data_handler](/cells/es/python-net/aspose.cells/odsloadoptions/light_cells_data_handler) | El controlador de datos para procesar datos de celdas al leer el archivo de plantilla.|
| [memory_setting](/cells/es/python-net/aspose.cells/odsloadoptions/memory_setting) | Obtiene o establece las opciones de uso de la memoria.|
| [warning_callback](/cells/es/python-net/aspose.cells/odsloadoptions/warning_callback) | Obtiene o establece una devolución de llamada de advertencia.|
| [auto_fitter_options](/cells/es/python-net/aspose.cells/odsloadoptions/auto_fitter_options) | Obtiene y establece las opciones de ajuste automático|
| [auto_filter](/cells/es/python-net/aspose.cells/odsloadoptions/auto_filter) | Indica si se filtran automáticamente los datos al cargar los archivos.|
| [font_configs](/cells/es/python-net/aspose.cells/odsloadoptions/font_configs) | Obtiene y establece configuraciones de fuentes individuales.<br/> Solo funciona para el [Workbook](/cells/es/python-net/aspose.cells/workbook) que usa este [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions) para cargar.|
| [apply_excel_default_style_to_hyperlink](/cells/es/python-net/aspose.cells/odsloadoptions/apply_excel_default_style_to_hyperlink) | Indica si se aplica el estilo predeterminado del Excel al hipervínculo.|
| [refresh_pivot_tables](/cells/es/python-net/aspose.cells/odsloadoptions/refresh_pivot_tables) | Indica si se actualizan las tablas dinámicas al cargar el archivo.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_paper_size(type)](/cells/es/python-net/aspose.cells/odsloadoptions/set_paper_size/#PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración predeterminada de la impresora.|



###  Ver también
* módulo [aspose.cells](..)
* clase [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)
* clase [OdsLoadOptions](/cells/es/python-net/aspose.cells/odsloadoptions)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
