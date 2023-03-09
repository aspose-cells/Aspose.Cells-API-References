---
title: HtmlLoadOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 770
url: /es/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  HtmlLoadOptions clase
Representa opciones al importar un archivo html.



**Herencia:** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)



El tipo HtmlLoadOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [HtmlLoadOptions()](/cells/es/python-net/aspose.cells/htmlloadoptions/__init__/#) | Crea una opción de cargar el archivo.|
| [HtmlLoadOptions(load_format)](/cells/es/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) | Crea una opción de cargar el archivo.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [load_format](/cells/es/python-net/aspose.cells/htmlloadoptions/load_format) | Obtiene el formato de carga.|
| [password](/cells/es/python-net/aspose.cells/htmlloadoptions/password) | Obtiene y establece la contraseña del libro.|
| [parsing_formula_on_open](/cells/es/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | Indica si se analiza la fórmula al leer el archivo.|
| [parsing_pivot_cached_records](/cells/es/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | Indica si se están analizando los registros en caché dinámicos al cargar el archivo.<br/> El valor predeterminado es falso.|
| [language_code](/cells/es/python-net/aspose.cells/htmlloadoptions/language_code) | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo en función del código de país que guardó el archivo.|
| [region](/cells/es/python-net/aspose.cells/htmlloadoptions/region) | Obtiene o establece la configuración regional del sistema según el código de país en el momento en que se cargó el archivo.|
| [default_style_settings](/cells/es/python-net/aspose.cells/htmlloadoptions/default_style_settings) | Obtiene la configuración de estilo predeterminada para inicializar estilos del libro de trabajo|
| [standard_font](/cells/es/python-net/aspose.cells/htmlloadoptions/standard_font) | Establece el nombre de fuente estándar predeterminado|
| [standard_font_size](/cells/es/python-net/aspose.cells/htmlloadoptions/standard_font_size) | Establece el tamaño de fuente estándar predeterminado.|
| [interrupt_monitor](/cells/es/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | Obtiene y establece el monitor de interrupciones.|
| [ignore_not_printed](/cells/es/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | Ignore los datos que no se imprimen si imprime directamente el archivo|
| [check_data_valid](/cells/es/python-net/aspose.cells/htmlloadoptions/check_data_valid) |Compruebe si los datos son válidos en el archivo de plantilla.|
| [check_excel_restriction](/cells/es/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas.<br/>Por ejemplo, Excel no permite ingresar un valor de cadena de más de 32K.<br/>Cuando ingresa un valor de más de 32 K, como Cell.PutValue (cadena), si esta propiedad es verdadera, obtendrá una excepción.<br/>Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego<br/>puede generar el valor de cadena completo para otros formatos de archivo como CSV.<br/>Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel,<br/> no debe guardar el libro de trabajo como formato de archivo de Excel más tarde.|
| [keep_unparsed_data](/cells/es/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) | Si se mantienen los datos no analizados en la memoria para el libro de trabajo cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.|
| [load_filter](/cells/es/python-net/aspose.cells/htmlloadoptions/load_filter) | El filtro para indicar cómo cargar datos.|
| [light_cells_data_handler](/cells/es/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | El controlador de datos para procesar datos de celdas al leer el archivo de plantilla.|
| [memory_setting](/cells/es/python-net/aspose.cells/htmlloadoptions/memory_setting) | Obtiene o establece las opciones de uso de la memoria.|
| [warning_callback](/cells/es/python-net/aspose.cells/htmlloadoptions/warning_callback) | Obtiene o establece devoluciones de llamada de advertencia.|
| [auto_fitter_options](/cells/es/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | Obtiene y establece las opciones de ajuste automático|
| [auto_filter](/cells/es/python-net/aspose.cells/htmlloadoptions/auto_filter) | Indica si se filtran automáticamente los datos al cargar los archivos.|
| [font_configs](/cells/es/python-net/aspose.cells/htmlloadoptions/font_configs) | Obtiene y establece configuraciones de fuentes individuales.<br/> Solo funciona para el [Workbook](/cells/es/python-net/aspose.cells/workbook) que usa este [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions) para cargar.|
| [encoding](/cells/es/python-net/aspose.cells/htmlloadoptions/encoding) | Obtiene y establece la codificación predeterminada.|
| [load_style_strategy](/cells/es/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |Indica la estrategia para aplicar estilo a los valores analizados al convertir el valor de cadena en número o fecha y hora.|
| [convert_numeric_data](/cells/es/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos numéricos.|
| [convert_date_time_data](/cells/es/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos de fecha.|
| [keep_precision](/cells/es/python-net/aspose.cells/htmlloadoptions/keep_precision) | Indica si no se analiza un valor de cadena si la longitud es 15.|
| [attached_files_directory](/cells/es/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | El directorio en el que se guardarán los archivos adjuntos.|
| [load_formulas](/cells/es/python-net/aspose.cells/htmlloadoptions/load_formulas) | Indica si se importan fórmulas si el archivo html original contiene fórmulas|
| [support_div_tag](/cells/es/python-net/aspose.cells/htmlloadoptions/support_div_tag) | Indica si admite el diseño de<div> etiqueta cuando el archivo html contiene<div> etiquetas|
| [delete_redundant_spaces](/cells/es/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | Indica si se eliminan los espacios redundantes cuando el texto se ajusta a las líneas usando<br> etiqueta El valor predeterminado es falso.|
| [auto_fit_cols_and_rows](/cells/es/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | Indica si las columnas y filas se ajustan automáticamente.|
| [convert_formulas_data](/cells/es/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | si es verdadero, convierta la cadena en fórmula cuando el valor de la cadena comience con el carácter '=', el valor predeterminado es falso.|
| [stream_provider](/cells/es/python-net/aspose.cells/htmlloadoptions/stream_provider) | Obtiene o establece StreamProviderImportHtmlFile para importar objetos.|
| [prog_id](/cells/es/python-net/aspose.cells/htmlloadoptions/prog_id) | Obtiene la identificación del programa de creación del archivo.<br/> Solo para archivos MHT.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_paper_size(type)](/cells/es/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración predeterminada de la impresora.|



###  Ver también
* módulo [aspose.cells](..)
* clase [AbstractTextLoadOptions](/cells/es/python-net/aspose.cells/abstracttextloadoptions)
* clase [HtmlLoadOptions](/cells/es/python-net/aspose.cells/htmlloadoptions)
* clase [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
