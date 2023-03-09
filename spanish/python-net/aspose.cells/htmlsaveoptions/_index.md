---
title: HtmlSaveOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 780
url: /es/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions clase
Representa las opciones para guardar el archivo html.



**Herencia:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)



El tipo HtmlSaveOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [HtmlSaveOptions()](/cells/es/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Crea opciones para guardar el archivo html.|
| [HtmlSaveOptions(format)](/cells/es/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Crea opciones para guardar el archivo htm.|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [save_format](/cells/es/python-net/aspose.cells/htmlsaveoptions/save_format) | Obtiene el formato de archivo guardado.|
| [clear_data](/cells/es/python-net/aspose.cells/htmlsaveoptions/clear_data) | Vacíe el libro de trabajo después de guardar el archivo.|
| [cached_file_folder](/cells/es/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño.|
| [validate_merged_areas](/cells/es/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Indica si validar las celdas combinadas antes de guardar el archivo.|
| [merge_areas](/cells/es/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo.|
| [create_directory](/cells/es/python-net/aspose.cells/htmlsaveoptions/create_directory) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.|
| [sort_names](/cells/es/python-net/aspose.cells/htmlsaveoptions/sort_names) | Indica si ordenar los nombres definidos antes de guardar el archivo.|
| [sort_external_names](/cells/es/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Indica si ordenar los nombres definidos externos antes de guardar el archivo.|
| [refresh_chart_cache](/cells/es/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) |Indica si se actualizan los datos de la memoria caché del gráfico|
| [warning_callback](/cells/es/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Obtiene o establece una devolución de llamada de advertencia.|
| [update_smart_art](/cells/es/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indica si se está actualizando la configuración de arte inteligente.<br/> El valor predeterminado es falso.|
| [ignore_invisible_shapes](/cells/es/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Indicar si exportar esas formas no visibles|
| [page_title](/cells/es/python-net/aspose.cells/htmlsaveoptions/page_title) | El título de la página html.<br/> Solo para guardar en flujo html.|
| [attached_files_directory](/cells/es/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) |El directorio en el que se guardarán los archivos adjuntos.<br/> Solo para guardar en flujo html.|
| [attached_files_url_prefix](/cells/es/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Especifique el prefijo de URL de los archivos adjuntos, como la imagen en el archivo html.<br/> Solo para guardar en flujo html.|
| [default_font_name](/cells/es/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Especifique el nombre de fuente predeterminado para exportar html, la fuente predeterminada se utilizará cuando la fuente de estilo no exista,<br/>Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tiene la misma familia que la fuente original,<br/> el valor predeterminado es nulo.|
| [worksheet_scalable](/cells/es/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) |Indica si acercar o alejar el html a través del nivel de zoom de la hoja de trabajo al guardar el archivo en html, el valor predeterminado es falso.|
| [is_export_comments](/cells/es/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indica si al exportar comentarios al guardar el archivo en html, el valor predeterminado es falso.|
| [export_comments_type](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Representa el tipo de exportación de comentarios a archivos html.|
| [disable_downlevel_revealed_comments](/cells/es/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indica si se deshabilitan los comentarios condicionales revelados por nivel inferior al exportar un archivo a html, el valor predeterminado es falso.|
| [is_exp_image_to_temp_dir](/cells/es/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Indica si se exportan archivos de imagen al directorio temporal.<br/> Solo para guardar en flujo html.|
| [image_scalable](/cells/es/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Indica si se utiliza una unidad escalable para describir el ancho de la imagen<br/>cuando se usa una unidad escalable para describir el ancho de la columna.<br/> El valor por defecto es verdadero.|
| [width_scalable](/cells/es/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Indica si se usa una unidad escalable para describir el ancho de columna al exportar un archivo a html.<br/> El valor predeterminado es falso.|
| [export_single_tab](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Indica si exportar la pestaña única cuando el archivo solo tiene una hoja de trabajo.<br/> El valor predeterminado es falso.|
| [export_images_as_base64](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB.|
| [export_active_worksheet_only](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indica si se exporta todo el libro de trabajo a un archivo html.|
| [export_print_area_only](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Indica si solo se exporta el área de impresión a un archivo html. El valor predeterminado es falso.|
| [export_area](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_area) | Obtiene o establece la exportación de CellArea de la hoja de trabajo activa actual.<br/>Si establece este atributo, se omitirá el área de impresión de la hoja de trabajo activa actual.<br/> Solo se exportará el área especificada al guardar el archivo en html.|
| [parse_html_tag_in_cell](/cells/es/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Analizar la etiqueta html en la celda, como valor de celda o como etiqueta html, el valor predeterminado es verdadero|
| [html_cross_string_type](/cells/es/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indica si una cadena de celdas cruzadas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato html.<br/>De forma predeterminada, el valor es Predeterminado, por lo que, para cadenas de celdas cruzadas, hay poca diferencia entre los archivos html creados por Aspose.Cells y MS Excel.<br/>Pero el rendimiento para crear archivos html grandes, establecer el valor en Cruz sería varias veces más rápido que establecerlo en Predeterminado o Fit2Cell.|
| [hidden_col_display_type](/cells/es/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardar esto en formato html,<br/>si HtmlHiddenColDisplayType es "Eliminar", la columna oculta no se generará,<br/> si el valor es "Oculto", la columna se mostraría, pero estaba oculta, el valor predeterminado es "Oculto"|
| [hidden_row_display_type](/cells/es/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardar esto en formato html,<br/>si HtmlHiddenRowDisplayType es "Eliminar", la fila oculta no se generará,<br/> si el valor es "Oculto", la fila se mostraría, pero estaba oculta, el valor predeterminado es "Oculto"|
| [encoding](/cells/es/python-net/aspose.cells/htmlsaveoptions/encoding) | Si no está configurado, use Codificación.UTF8 como tipo de codificación predeterminado.|
| [export_object_listener](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Obtiene o establece ExportObjectListener para exportar objetos.|
| [file_path_provider](/cells/es/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Obtiene o establece el IFilePathProvider para exportar la hoja de trabajo a html por separado.|
| [stream_provider](/cells/es/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Obtiene o establece IStreamProvider para exportar objetos.|
| [image_options](/cells/es/python-net/aspose.cells/htmlsaveoptions/image_options) | Obtenga el objeto ImageOrPrintOptions antes de exportar|
| [save_as_single_file](/cells/es/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Indica si guardar el html como archivo único.<br/> El valor predeterminado es falso.|
| [show_all_sheets](/cells/es/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Indica si se muestran todas las hojas al guardarlas como un solo archivo html.|
| [export_page_headers](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Indica si se exportan encabezados de página.|
| [export_page_footers](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Indica si se exportan encabezados de página.|
| [export_hidden_worksheet](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Indica si se exporta el contenido oculto de la hoja de trabajo. El valor predeterminado es verdadero.|
| [presentation_preference](/cells/es/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indicando si el archivo html o mht es la preferencia de presentación.<br/>El valor predeterminado es falso.<br/> Si desea obtener una presentación más hermosa, establezca el valor en verdadero.|
| [cell_css_prefix](/cells/es/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Obtiene y establece el prefijo del nombre css, el valor predeterminado es "".|
| [table_css_id](/cells/es/python-net/aspose.cells/htmlsaveoptions/table_css_id) |Obtiene y establece el prefijo del nombre de tipo css, como tr, col, td, etc., están contenidos en el elemento de la tabla<br/> que tiene el atributo TableCssId específico. El valor predeterminado es "".|
| [is_full_path_link](/cells/es/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Indicando si se usa el enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm.<br/> El valor predeterminado es falso.|
| [export_worksheet_css_separately](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Indicando si exportar la hoja de trabajo css por separado. El valor predeterminado es falso.|
| [export_similar_border_style](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Indicar si se exporta el estilo de borde similar cuando los navegadores no admiten el estilo de borde.<br/>Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.<br/> El valor predeterminado es falso.|
| [merge_empty_td_forcely](/cells/es/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indica si se fusiona el elemento TD vacío a la fuerza al exportar el archivo a html.<br/> El tamaño del archivo html se reducirá significativamente después de establecer el valor en verdadero. El valor predeterminado es falso.<br/> Si desea importar el archivo html para sobresalir o exportar líneas de cuadrícula perfectas al guardar el archivo en html,<br/> por favor, mantenga el valor predeterminado.|
| [export_cell_coordinate](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Indica si se exporta la coordenada de Excel de las celdas que no están en blanco al guardar el archivo en html. El valor predeterminado es falso.<br/> Si desea importar el html de salida a Excel, mantenga el valor predeterminado.|
| [export_extra_headings](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Indica si se exportan encabezados adicionales cuando la longitud del texto es más larga que la columna de visualización máxima.<br/> El valor predeterminado es falso. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.|
| [export_headings](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_headings) | Indica si se exportan los encabezados de fila y columna de la hoja al guardar en archivos HTML.|
| [export_row_column_headings](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Indica si se exportan los encabezados de fila y columna de la hoja al guardar en archivos HTML.|
| [export_formula](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_formula) | Indica si se exporta la fórmula al guardar el archivo en html. El valor por defecto es verdadero.<br/> Si desea importar el html de salida a Excel, mantenga el valor predeterminado.|
| [add_tooltip_text](/cells/es/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) |Indica si se agrega texto de información sobre herramientas cuando los datos no se pueden mostrar por completo.<br/> El valor predeterminado es falso.|
| [export_grid_lines](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Indicando si se exportan las líneas de cuadrícula. El valor predeterminado es falso.|
| [export_bogus_row_data](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es verdadero. Si desea importar el archivo html o mht<br/> para sobresalir, mantenga el valor predeterminado.|
| [exclude_unused_styles](/cells/es/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Indicando si excluye estilos no utilizados.<br/>Para los archivos html generados, la exclusión de estilos no utilizados puede reducir el tamaño del archivo.<br/>sin afectar los efectos visuales. Entonces, el valor predeterminado de esta propiedad es verdadero.<br/>Si el usuario necesita mantener todos los estilos en el libro de trabajo para el html generado (como el escenario en el que el usuario<br/> necesita restaurar el libro de trabajo desde el html generado más tarde), establezca esta propiedad como falsa.|
| [export_document_properties](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Indicando si exporta propiedades del documento. El valor por defecto es verdadero. Si desea importar<br/> el archivo html o mht para sobresalir, mantenga el valor predeterminado.|
| [export_worksheet_properties](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Indicando si se exportan las propiedades de la hoja de trabajo. El valor predeterminado es verdadero. Si desea importar<br/> el archivo html o mht para sobresalir, mantenga el valor predeterminado.|
| [export_workbook_properties](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Indicando si se están exportando las propiedades del libro. El valor predeterminado es verdadero. Si desea importar<br/> el archivo html o mht para sobresalir, mantenga el valor predeterminado.|
| [export_frame_scripts_and_properties](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Indicando si se exportan secuencias de comandos de fotogramas y propiedades del documento. El valor predeterminado es verdadero. Si desea importar el archivo html o mht<br/> para sobresalir, mantenga el valor predeterminado.|
| [export_data_options](/cells/es/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indica la regla de exportación de datos de archivos html. El valor predeterminado es Todo.|
| [link_target_type](/cells/es/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Indicar el tipo de atributo de destino en<a> enlace, el valor predeterminado es HtmlLinkTargetType.Parent.|



###  Ver también
* módulo [aspose.cells](..)
* clase [HtmlSaveOptions](/cells/es/python-net/aspose.cells/htmlsaveoptions)
* clase [SaveOptions](/cells/es/python-net/aspose.cells/saveoptions)
