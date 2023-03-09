---
title: PptxSaveOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1190
url: /es/python-net/aspose.cells/pptxsaveoptions/
is_root: false
---
##  PptxSaveOptions clase
Representa las opciones de guardado de pptx.



**Herencia:** [PptxSaveOptions](/cells/python-net/aspose.cells/pptxsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)



El tipo PptxSaveOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [PptxSaveOptions()](/cells/es/python-net/aspose.cells/pptxsaveoptions/__init__/#) | Representa las opciones de guardado de pptx.|
| [PptxSaveOptions(save_as_image)](/cells/es/python-net/aspose.cells/pptxsaveoptions/__init__/#bool) | Representa las opciones para guardar el archivo .pptx.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells/pptxsaveoptions/save_format) | Obtiene el formato de archivo guardado.|
| [clear_data](/cells/es/python-net/aspose.cells/pptxsaveoptions/clear_data) | Vacíe el libro de trabajo después de guardar el archivo.|
| [cached_file_folder](/cells/es/python-net/aspose.cells/pptxsaveoptions/cached_file_folder) | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño.|
| [validate_merged_areas](/cells/es/python-net/aspose.cells/pptxsaveoptions/validate_merged_areas) | Indica si validar las celdas combinadas antes de guardar el archivo.|
| [merge_areas](/cells/es/python-net/aspose.cells/pptxsaveoptions/merge_areas) | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo.|
| [create_directory](/cells/es/python-net/aspose.cells/pptxsaveoptions/create_directory) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.|
| [sort_names](/cells/es/python-net/aspose.cells/pptxsaveoptions/sort_names) | Indica si ordenar los nombres definidos antes de guardar el archivo.|
| [sort_external_names](/cells/es/python-net/aspose.cells/pptxsaveoptions/sort_external_names) |Indica si ordenar los nombres definidos externamente antes de guardar el archivo.|
| [refresh_chart_cache](/cells/es/python-net/aspose.cells/pptxsaveoptions/refresh_chart_cache) | Indica si se actualizan los datos de la memoria caché del gráfico|
| [warning_callback](/cells/es/python-net/aspose.cells/pptxsaveoptions/warning_callback) | Obtiene o establece devoluciones de llamada de advertencia.|
| [update_smart_art](/cells/es/python-net/aspose.cells/pptxsaveoptions/update_smart_art) | Indica si se está actualizando la configuración de arte inteligente.<br/> El valor predeterminado es falso.|
| [default_font](/cells/es/python-net/aspose.cells/pptxsaveoptions/default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/>Establezca DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres.<br/> Si no se establece esta propiedad, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.|
| [check_workbook_default_font](/cells/es/python-net/aspose.cells/pptxsaveoptions/check_workbook_default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/> Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero.|
| [check_font_compatibility](/cells/es/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility) |Indica si se debe comprobar la compatibilidad de fuentes para cada carácter del texto.|
| [is_font_substitution_char_granularity](/cells/es/python-net/aspose.cells/pptxsaveoptions/is_font_substitution_char_granularity) | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él.|
| [one_page_per_sheet](/cells/es/python-net/aspose.cells/pptxsaveoptions/one_page_per_sheet) | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado.<br/> El tamaño de papel de configuración de página no será válido, y las otras configuraciones de configuración de página<br/> aún tendrá efecto.|
| [all_columns_in_one_page_per_sheet](/cells/es/python-net/aspose.cells/pptxsaveoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado.<br/> Se ignorará el ancho del tamaño del papel de la configuración de la página, y las demás configuraciones de la configuración de la página<br/> aún tendrá efecto.|
| [ignore_error](/cells/es/python-net/aspose.cells/pptxsaveoptions/ignore_error) | Indica si necesita ocultar el error durante el renderizado.<br/> El error puede ser un error en la forma, la imagen, la representación del gráfico, etc.|
| [output_blank_page_when_nothing_to_print](/cells/es/python-net/aspose.cells/pptxsaveoptions/output_blank_page_when_nothing_to_print) | Indica si imprimir una página en blanco cuando no hay nada que imprimir.|
| [page_index](/cells/es/python-net/aspose.cells/pptxsaveoptions/page_index) | Obtiene o establece el índice basado en 0 de la primera página que se va a guardar.|
| [page_count](/cells/es/python-net/aspose.cells/pptxsaveoptions/page_count) | Obtiene o establece el número de páginas que se van a guardar.|
| [printing_page_type](/cells/es/python-net/aspose.cells/pptxsaveoptions/printing_page_type) | Indica qué páginas no se imprimirán.|
| [gridline_type](/cells/es/python-net/aspose.cells/pptxsaveoptions/gridline_type) | Obtiene o establece el tipo de línea de cuadrícula.|
| [text_cross_type](/cells/es/python-net/aspose.cells/pptxsaveoptions/text_cross_type) | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda.|
| [default_edit_language](/cells/es/python-net/aspose.cells/pptxsaveoptions/default_edit_language) | Obtiene o establece el idioma de edición predeterminado.|
| [sheet_set](/cells/es/python-net/aspose.cells/pptxsaveoptions/sheet_set) |Obtiene o establece las hojas para representar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [SheetSet.visible](/cells/es/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/es/python-net/aspose.cells/pptxsaveoptions/draw_object_event_handler) | Implementa esta interfaz para obtener DrawObject y Bound al renderizar.|
| [page_saving_callback](/cells/es/python-net/aspose.cells/pptxsaveoptions/page_saving_callback) | Controlar/Indicar el progreso del proceso de guardado de la página.|



###  Ver también
* módulo [aspose.cells](..)
* clase [PaginatedSaveOptions](/cells/es/python-net/aspose.cells/paginatedsaveoptions)
* clase [PptxSaveOptions](/cells/es/python-net/aspose.cells/pptxsaveoptions)
* clase [SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)
