---
title: PaginatedSaveOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1150
url: /es/python-net/aspose.cells/paginatedsaveoptions/
is_root: false
---
##  PaginatedSaveOptions clase
Representa las opciones de paginación.



**Herencia:** [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)



El tipo PaginatedSaveOptions expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells/paginatedsaveoptions/save_format) | Obtiene el formato de archivo guardado.|
| [clear_data](/cells/es/python-net/aspose.cells/paginatedsaveoptions/clear_data) | Vacíe el libro de trabajo después de guardar el archivo.|
| [cached_file_folder](/cells/es/python-net/aspose.cells/paginatedsaveoptions/cached_file_folder) | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño.|
| [validate_merged_areas](/cells/es/python-net/aspose.cells/paginatedsaveoptions/validate_merged_areas) | Indica si validar las celdas combinadas antes de guardar el archivo.|
| [merge_areas](/cells/es/python-net/aspose.cells/paginatedsaveoptions/merge_areas) | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo.|
| [create_directory](/cells/es/python-net/aspose.cells/paginatedsaveoptions/create_directory) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.|
| [sort_names](/cells/es/python-net/aspose.cells/paginatedsaveoptions/sort_names) | Indica si ordenar los nombres definidos antes de guardar el archivo.|
| [sort_external_names](/cells/es/python-net/aspose.cells/paginatedsaveoptions/sort_external_names) | Indica si ordenar los nombres definidos externos antes de guardar el archivo.|
| [refresh_chart_cache](/cells/es/python-net/aspose.cells/paginatedsaveoptions/refresh_chart_cache) |Indica si se actualizan los datos de la memoria caché del gráfico|
| [warning_callback](/cells/es/python-net/aspose.cells/paginatedsaveoptions/warning_callback) | Obtiene o establece una devolución de llamada de advertencia.|
| [update_smart_art](/cells/es/python-net/aspose.cells/paginatedsaveoptions/update_smart_art) | Indica si se está actualizando la configuración de arte inteligente.<br/> El valor predeterminado es falso.|
| [default_font](/cells/es/python-net/aspose.cells/paginatedsaveoptions/default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/>Establezca DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres.<br/> Si no se establece esta propiedad, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.|
| [check_workbook_default_font](/cells/es/python-net/aspose.cells/paginatedsaveoptions/check_workbook_default_font) | Cuando los caracteres en Excel son Unicode y no se configuran con la fuente correcta en el estilo de celda,<br/>Pueden aparecer como bloque en pdf, imagen.<br/> Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero.|
| [check_font_compatibility](/cells/es/python-net/aspose.cells/paginatedsaveoptions/check_font_compatibility) | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter del texto.|
| [is_font_substitution_char_granularity](/cells/es/python-net/aspose.cells/paginatedsaveoptions/is_font_substitution_char_granularity) | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él.|
| [one_page_per_sheet](/cells/es/python-net/aspose.cells/paginatedsaveoptions/one_page_per_sheet) | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado.<br/> El tamaño de papel de configuración de página no será válido, y las otras configuraciones de configuración de página<br/> aún tendrá efecto.|
| [all_columns_in_one_page_per_sheet](/cells/es/python-net/aspose.cells/paginatedsaveoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado.<br/> Se ignorará el ancho del tamaño del papel de la configuración de la página, y las demás configuraciones de la configuración de la página<br/> aún tendrá efecto.|
| [ignore_error](/cells/es/python-net/aspose.cells/paginatedsaveoptions/ignore_error) | Indica si necesita ocultar el error durante el renderizado.<br/> El error puede ser un error en la forma, la imagen, la representación del gráfico, etc.|
| [output_blank_page_when_nothing_to_print](/cells/es/python-net/aspose.cells/paginatedsaveoptions/output_blank_page_when_nothing_to_print) | Indica si imprimir una página en blanco cuando no hay nada que imprimir.|
| [page_index](/cells/es/python-net/aspose.cells/paginatedsaveoptions/page_index) | Obtiene o establece el índice basado en 0 de la primera página que se va a guardar.|
| [page_count](/cells/es/python-net/aspose.cells/paginatedsaveoptions/page_count) | Obtiene o establece el número de páginas que se van a guardar.|
| [printing_page_type](/cells/es/python-net/aspose.cells/paginatedsaveoptions/printing_page_type) | Indica qué páginas no se imprimirán.|
| [gridline_type](/cells/es/python-net/aspose.cells/paginatedsaveoptions/gridline_type) | Obtiene o establece el tipo de línea de cuadrícula.|
| [text_cross_type](/cells/es/python-net/aspose.cells/paginatedsaveoptions/text_cross_type) | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda.|
| [default_edit_language](/cells/es/python-net/aspose.cells/paginatedsaveoptions/default_edit_language) | Obtiene o establece el idioma de edición predeterminado.|
| [sheet_set](/cells/es/python-net/aspose.cells/paginatedsaveoptions/sheet_set) |Obtiene o establece las hojas para representar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [SheetSet.visible](/cells/es/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/es/python-net/aspose.cells/paginatedsaveoptions/draw_object_event_handler) | Implementa esta interfaz para obtener DrawObject y Bound al renderizar.|
| [page_saving_callback](/cells/es/python-net/aspose.cells/paginatedsaveoptions/page_saving_callback) |Controlar/Indicar el progreso del proceso de guardado de la página.|



###  Ver también
* módulo [aspose.cells](..)
* clase [PaginatedSaveOptions](/cells/es/python-net/aspose.cells/paginatedsaveoptions)
* clase [SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)
