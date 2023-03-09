---
title: TxtLoadOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1510
url: /es/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  TxtLoadOptions clase
Representa las opciones para cargar el archivo de texto.



**Herencia:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)



El tipo TxtLoadOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [TxtLoadOptions()](/cells/es/python-net/aspose.cells/txtloadoptions/__init__/#) | Crea las opciones para cargar el archivo de texto.|
| [TxtLoadOptions(load_format)](/cells/es/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | Crea las opciones para cargar el archivo de texto.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [load_format](/cells/es/python-net/aspose.cells/txtloadoptions/load_format) | Obtiene el formato de carga.|
| [password](/cells/es/python-net/aspose.cells/txtloadoptions/password) | Obtiene y establece la contraseña del libro de trabajo.|
| [parsing_formula_on_open](/cells/es/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Indica si se analiza la fórmula al leer el archivo.|
| [parsing_pivot_cached_records](/cells/es/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Indica si se están analizando los registros en caché dinámicos al cargar el archivo.<br/> El valor predeterminado es falso.|
| [language_code](/cells/es/python-net/aspose.cells/txtloadoptions/language_code) | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo en función del código de país que guardó el archivo.|
| [region](/cells/es/python-net/aspose.cells/txtloadoptions/region) | Obtiene o establece la configuración regional del sistema según el código de país en el momento en que se cargó el archivo.|
| [default_style_settings](/cells/es/python-net/aspose.cells/txtloadoptions/default_style_settings) | Obtiene la configuración de estilo predeterminada para inicializar estilos del libro de trabajo|
| [standard_font](/cells/es/python-net/aspose.cells/txtloadoptions/standard_font) | Establece el nombre de fuente estándar predeterminado|
| [standard_font_size](/cells/es/python-net/aspose.cells/txtloadoptions/standard_font_size) | Establece el tamaño de fuente estándar predeterminado.|
| [interrupt_monitor](/cells/es/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Obtiene y establece el monitor de interrupciones.|
| [ignore_not_printed](/cells/es/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignore los datos que no se imprimen si imprime directamente el archivo|
| [check_data_valid](/cells/es/python-net/aspose.cells/txtloadoptions/check_data_valid) | Compruebe si los datos son válidos en el archivo de plantilla.|
| [check_excel_restriction](/cells/es/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas.<br/>Por ejemplo, Excel no permite ingresar un valor de cadena de más de 32K.<br/>Cuando ingresa un valor de más de 32 K, como Cell.PutValue (cadena), si esta propiedad es verdadera, obtendrá una excepción.<br/>Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego<br/>puede generar el valor de cadena completo para otros formatos de archivo como CSV.<br/>Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel,<br/> no debe guardar el libro de trabajo como formato de archivo de Excel más tarde. De lo contrario, puede haber un error inesperado para el archivo de Excel generado.|
| [keep_unparsed_data](/cells/es/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) |Si mantiene los datos no analizados en la memoria para el libro de trabajo cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.|
| [load_filter](/cells/es/python-net/aspose.cells/txtloadoptions/load_filter) | El filtro para indicar cómo cargar datos.|
| [light_cells_data_handler](/cells/es/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | El controlador de datos para procesar datos de celdas al leer el archivo de plantilla.|
| [memory_setting](/cells/es/python-net/aspose.cells/txtloadoptions/memory_setting) | Obtiene o establece las opciones de uso de la memoria.|
| [warning_callback](/cells/es/python-net/aspose.cells/txtloadoptions/warning_callback) | Obtiene o establece una devolución de llamada de advertencia.|
| [auto_fitter_options](/cells/es/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Obtiene y establece las opciones de ajuste automático|
| [auto_filter](/cells/es/python-net/aspose.cells/txtloadoptions/auto_filter) | Indica si se filtran automáticamente los datos al cargar los archivos.|
| [font_configs](/cells/es/python-net/aspose.cells/txtloadoptions/font_configs) | Obtiene y establece configuraciones de fuentes individuales.<br/> Solo funciona para el [Workbook](/cells/es/python-net/aspose.cells/workbook) que usa este [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions) para cargar.|
| [encoding](/cells/es/python-net/aspose.cells/txtloadoptions/encoding) | Obtiene y establece la codificación predeterminada. Solo aplica para archivo csv.|
| [load_style_strategy](/cells/es/python-net/aspose.cells/txtloadoptions/load_style_strategy) |Indica la estrategia para aplicar estilo a los valores analizados al convertir el valor de cadena en número o fecha y hora.|
| [convert_numeric_data](/cells/es/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos numéricos.|
| [convert_date_time_data](/cells/es/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos de fecha.|
| [keep_precision](/cells/es/python-net/aspose.cells/txtloadoptions/keep_precision) | Indica si no se analiza un valor de cadena si la longitud es 15.|
| [separator](/cells/es/python-net/aspose.cells/txtloadoptions/separator) |Obtiene y establece el separador de caracteres del archivo de texto.|
| [separator_string](/cells/es/python-net/aspose.cells/txtloadoptions/separator_string) | Obtiene y establece un valor de cadena como separador.|
| [is_multi_encoded](/cells/es/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | Verdadero significa que el archivo contiene varias codificaciones.|
| [preferred_parsers](/cells/es/python-net/aspose.cells/txtloadoptions/preferred_parsers) | Obtiene y establece los analizadores de valores preferidos para cargar archivos de texto.|
| [has_formula](/cells/es/python-net/aspose.cells/txtloadoptions/has_formula) | Indica si el texto es fórmula si comienza con "=".|
| [has_text_qualifier](/cells/es/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Si hay un calificador de texto para el valor de la celda. El valor predeterminado es verdadero.|
| [text_qualifier](/cells/es/python-net/aspose.cells/txtloadoptions/text_qualifier) | Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '"'.|
| [treat_consecutive_delimiters_as_one](/cells/es/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) |Si los delimitadores consecutivos deben tratarse como uno solo.|
| [treat_quote_prefix_as_value](/cells/es/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) |Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda.<br/>El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente<br/> y [Style.quote_prefix](/cells/es/python-net/aspose.cells/style#quote_prefix) se configurará como verdadero para la celda.|
| [extend_to_next_sheet](/cells/es/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Si extiende los datos a la siguiente hoja cuando las filas o columnas de datos superan el límite.<br/>Si esta propiedad es verdadera, los datos adicionales se extenderán a la siguiente hoja detrás de la actual (si la hoja actual es la última,<br/>se agregará una hoja nueva al libro de trabajo actual).<br/>Si esta propiedad es falsa, se ignorarán los datos que excedan el límite.<br/> El valor predeterminado es falso;|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_paper_size(type)](/cells/es/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración predeterminada de la impresora.|



###  Ver también
* módulo [aspose.cells](..)
* clase [AbstractTextLoadOptions](/cells/es/python-net/aspose.cells/abstracttextloadoptions)
* clase [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions)
* clase [TxtLoadOptions](/cells/es/python-net/aspose.cells/txtloadoptions)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
