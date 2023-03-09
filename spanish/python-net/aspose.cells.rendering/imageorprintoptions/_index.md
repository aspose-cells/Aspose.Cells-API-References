---
title: ImageOrPrintOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions clase
Permite especificar opciones al representar la hoja de trabajo en imágenes, imprimir la hoja de trabajo o representar el gráfico en la imagen.



El tipo ImageOrPrintOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [ImageOrPrintOptions()](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Construye una nueva instancia de ImageOrPrintOptions|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Obtiene o establece el tipo de formato de archivo de salida<br/> Soporte Tiff/XPS|
| [print_with_status_dialog](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Si PrintWithStatusDialog = true, habrá un cuadro de diálogo que muestra el estado de impresión actual.<br/> de lo contrario, no se mostrará dicho diálogo.|
| [horizontal_resolution](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) | Obtiene o establece la resolución horizontal de las imágenes generadas, en puntos por pulgada.<br/> Aplica el método de generación de imágenes, excepto las imágenes en formato Emf.|
| [vertical_resolution](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Obtiene o establece la resolución vertical de las imágenes generadas, en puntos por pulgada.<br/> Aplica el método de generación de imágenes, excepto la imagen en formato Emf.|
| [tiff_compression](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Obtiene o establece el tipo de compresión que se aplica solo cuando se guardan páginas en el formato `Tiff`.|
| [tiff_color_depth](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Obtiene o establece la profundidad de bits para que se aplique solo al guardar páginas en el formato `Tiff`.|
| [printing_page](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Indica qué páginas no se imprimirán.|
| [quality](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Obtiene o establece un valor que determina la calidad de las imágenes generadas<br/>para aplicar solo al guardar páginas en el formato `Jpeg`.|
| [image_type](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Obtiene o establece el formato de las imágenes generadas.<br/> valor predeterminado: PNG.|
| [is_cell_auto_fit](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Indica si el ancho y el alto de las celdas se ajustan automáticamente por valor de celda.<br/> El valor predeterminado es falso.|
| [one_page_per_sheet](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado.<br/> El tamaño de papel de configuración de página no será válido, y las otras configuraciones de configuración de página<br/> aún tendrá efecto.|
| [all_columns_in_one_page_per_sheet](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado.<br/> El ancho del tamaño del papel de la configuración de la página no será válido, y las demás configuraciones de la configuración de la página<br/> aún tendrá efecto.|
| [draw_object_event_handler](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Implementa esta interfaz para obtener DrawObject y Bound al renderizar.|
| [chart_image_type](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Indique el tipo de imagen del gráfico al convertir.<br/> valor predeterminado: PNG.|
| [embeded_image_name_in_svg](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Indique el nombre de archivo de la imagen incrustada en svg.<br/> Esta debería ser la ruta completa con un directorio como "c:\\xpsEmbedded"|
| [svg_fit_to_view_port](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | si esta propiedad es verdadera, el svg generado se ajustará al puerto de visualización.|
| [only_area](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Si esta propiedad es verdadera, se generará un área y no tendrá efecto ninguna escala.|
| [text_rendering_hint](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Especifica la calidad de la representación del texto.<br/> El valor predeterminado es TextRenderingHint.|
| [smoothing_mode](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Especifica si se aplica suavizado (antialiasing) a las líneas y curvas y los bordes de las áreas rellenas.<br/> El valor predeterminado es SmoothingMode.Ninguno|
| [transparent](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Indica si el fondo de la imagen generada debe ser transparente.|
| [pixel_format](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) |Obtiene o establece el formato de píxeles de las imágenes generadas.|
| [warning_callback](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Obtiene o establece devoluciones de llamada de advertencia.|
| [page_saving_callback](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) | Controlar/Indicar el progreso del proceso de guardado de la página.|
| [is_font_substitution_char_granularity](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él.|
| [page_index](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Obtiene o establece el índice basado en 0 de la primera página que se va a guardar.|
| [page_count](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Obtiene o establece el número de páginas que se van a guardar.|
| [is_optimized](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Indica si optimizar los elementos de salida.|
| [default_font](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/>Establezca DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres.<br/> Si no se establece esta propiedad, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.|
| [check_workbook_default_font](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/> Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero.|
| [output_blank_page_when_nothing_to_print](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Indica si imprimir una página en blanco cuando no hay nada que imprimir.|
| [gridline_type](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Obtiene o establece el tipo de línea de cuadrícula.|
| [text_cross_type](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda.|
| [emf_type](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Obtiene o establece un EmfType que especifica el formato del metarchivo.<br/> El valor predeterminado es EmfPlusDual.|
| [default_edit_language](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Obtiene o establece el idioma de edición predeterminado.|
| [sheet_set](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Obtiene o establece las hojas para representar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [SheetSet.visible](/cells/es/python-net/aspose.cells.rendering/sheetset#visible).|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/es/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Establece el ancho y alto deseados de la imagen.|



###  Ejemplos

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Ver también
* módulo [aspose.cells.rendering](..)
