---
title: PdfSaveOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1180
url: /es/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions clase
Representa las opciones para guardar archivos pdf.



**Herencia:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)



El tipo PdfSaveOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [PdfSaveOptions()](/cells/es/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Crea las opciones para guardar archivos pdf.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells/pdfsaveoptions/save_format) | Obtiene el formato de archivo guardado.|
| [clear_data](/cells/es/python-net/aspose.cells/pdfsaveoptions/clear_data) | Vacíe el libro de trabajo después de guardar el archivo.|
| [cached_file_folder](/cells/es/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño.|
| [validate_merged_areas](/cells/es/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Indica si validar las celdas combinadas antes de guardar el archivo.|
| [merge_areas](/cells/es/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo.|
| [create_directory](/cells/es/python-net/aspose.cells/pdfsaveoptions/create_directory) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.|
| [sort_names](/cells/es/python-net/aspose.cells/pdfsaveoptions/sort_names) | Indica si ordenar los nombres definidos antes de guardar el archivo.|
| [sort_external_names](/cells/es/python-net/aspose.cells/pdfsaveoptions/sort_external_names) |Indica si ordenar los nombres definidos externamente antes de guardar el archivo.|
| [refresh_chart_cache](/cells/es/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) | Indica si se actualizan los datos de la memoria caché del gráfico|
| [warning_callback](/cells/es/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Obtiene o establece devoluciones de llamada de advertencia.|
| [update_smart_art](/cells/es/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Indica si se está actualizando la configuración de arte inteligente.<br/> El valor predeterminado es falso.|
| [default_font](/cells/es/python-net/aspose.cells/pdfsaveoptions/default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/>Establezca DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres.<br/> Si no se establece esta propiedad, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.|
| [check_workbook_default_font](/cells/es/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/> Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero.|
| [check_font_compatibility](/cells/es/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) |Indica si se debe comprobar la compatibilidad de fuentes para cada carácter del texto.|
| [is_font_substitution_char_granularity](/cells/es/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él.|
| [one_page_per_sheet](/cells/es/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado.<br/> El tamaño de papel de configuración de página no será válido, y las otras configuraciones de configuración de página<br/> aún tendrá efecto.|
| [all_columns_in_one_page_per_sheet](/cells/es/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado.<br/> Se ignorará el ancho del tamaño del papel de la configuración de la página, y las demás configuraciones de la configuración de la página<br/> aún tendrá efecto.|
| [ignore_error](/cells/es/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Indica si necesita ocultar el error durante el renderizado.<br/> El error puede ser un error en la forma, la imagen, la representación del gráfico, etc.|
| [output_blank_page_when_nothing_to_print](/cells/es/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Indica si imprimir una página en blanco cuando no hay nada que imprimir.|
| [page_index](/cells/es/python-net/aspose.cells/pdfsaveoptions/page_index) | Obtiene o establece el índice basado en 0 de la primera página que se va a guardar.|
| [page_count](/cells/es/python-net/aspose.cells/pdfsaveoptions/page_count) | Obtiene o establece el número de páginas que se van a guardar.|
| [printing_page_type](/cells/es/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Indica qué páginas no se imprimirán.|
| [gridline_type](/cells/es/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Obtiene o establece el tipo de línea de cuadrícula.|
| [text_cross_type](/cells/es/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda.|
| [default_edit_language](/cells/es/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Obtiene o establece el idioma de edición predeterminado.|
| [sheet_set](/cells/es/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Obtiene o establece las hojas para representar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [SheetSet.visible](/cells/es/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/es/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implementa esta interfaz para obtener DrawObject y Bound al renderizar.|
| [page_saving_callback](/cells/es/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) | Controlar/Indicar el progreso del proceso de guardado de la página.|
| [embed_standard_windows_fonts](/cells/es/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True para incrustar fuentes de tipo verdadero.<br/>Afecta solo a los caracteres ASCII 32-127.<br/>Las fuentes para códigos de caracteres superiores a 127 siempre están incrustadas.<br/>Las fuentes siempre están incrustadas para el estándar PDF/A-1a, PDF/A-1b.<br/> El valor predeterminado es verdadero.|
| [bookmark](/cells/es/python-net/aspose.cells/pdfsaveoptions/bookmark) |Obtiene y establece el objeto [PdfBookmarkEntry](/cells/es/python-net/aspose.cells.rendering/pdfbookmarkentry).|
| [compliance](/cells/es/python-net/aspose.cells/pdfsaveoptions/compliance) | El libro de trabajo se convierte a pdf de acuerdo con PdfCompliance en esta propiedad.|
| [security_options](/cells/es/python-net/aspose.cells/pdfsaveoptions/security_options) | Establezca estas opciones cuando se necesite seguridad en el resultado xls2pdf.|
| [image_type](/cells/es/python-net/aspose.cells/pdfsaveoptions/image_type) | Representa el tipo de imagen al convertir el gráfico y la forma.|
| [calculate_formula](/cells/es/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Indica si calcular fórmulas antes de guardar el archivo pdf.|
| [pdf_compression](/cells/es/python-net/aspose.cells/pdfsaveoptions/pdf_compression) | Indicar el algoritmo de compresión|
| [created_time](/cells/es/python-net/aspose.cells/pdfsaveoptions/created_time) | Obtiene y establece la hora de generación del documento pdf.|
| [producer](/cells/es/python-net/aspose.cells/pdfsaveoptions/producer) | Obtiene y establece el productor del documento pdf generado.|
| [optimization_type](/cells/es/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Obtiene y establece el tipo de optimización de pdf.|
| [custom_properties_export](/cells/es/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Obtiene o establece un valor que determina la forma en que se exportan [CustomDocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection) al archivo PDF. El valor predeterminado es Ninguno.|
| [export_document_structure](/cells/es/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Indica si exportar la estructura del documento.|
| [emf_render_setting](/cells/es/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Configuración para renderizar el metarchivo Emf.|
| [display_doc_title](/cells/es/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Indica si la barra de título de la ventana debe mostrar el título del documento.|
| [font_encoding](/cells/es/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Obtiene o establece la codificación de fuentes incrustadas en pdf.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/es/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Establece los PPI (píxeles por pulgada) deseados de las imágenes de remuestreo y la calidad jpeg.<br/> Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada,<br/> las imágenes que superen los PPI (píxeles por pulgada) especificados se volverán a muestrear.|



###  Ver también
* módulo [aspose.cells](..)
* clase [CustomDocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection)
* clase [PaginatedSaveOptions](/cells/es/python-net/aspose.cells/paginatedsaveoptions)
* clase [PdfBookmarkEntry](/cells/es/python-net/aspose.cells.rendering/pdfbookmarkentry)
* clase [PdfSaveOptions](/cells/es/python-net/aspose.cells/pdfsaveoptions)
* clase [SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)
