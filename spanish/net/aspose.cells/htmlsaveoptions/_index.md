---
title: HtmlSaveOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa las opciones para guardar el archivo html.
type: docs
weight: 3740
url: /es/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Representa las opciones para guardar el archivo html.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Crea opciones para guardar el archivo html. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Crea opciones para guardar el archivo htm. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Indica si se agrega texto de información sobre herramientas cuando los datos no se pueden mostrar por completo. El valor predeterminado es false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | El directorio en el que se guardarán los archivos adjuntos. Solo para guardar en flujo html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Especifique el prefijo de URL de los archivos adjuntos, como la imagen en el archivo html. Solo para guardar en flujo html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Obtiene y establece el prefijo del nombre css, el valor predeterminado es "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Vacía el libro de trabajo después de guardar el archivo. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Especifique el nombre de la fuente predeterminada para exportar html, la fuente predeterminada se usará cuando la fuente del estilo no exista, Si esta propiedad es nula, Aspose.Cells usará la fuente universal que tiene la misma familia que la fuente original, el valor predeterminado es nulo. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Indica si se deshabilitan los comentarios condicionales revelados por nivel inferior al exportar un archivo a html, el valor predeterminado es falso. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Si no se establece, use Codificación.UTF8 como tipo de codificación predeterminado. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Indica si se excluyen estilos no utilizados. Para los archivos html generados, la exclusión de estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Entonces, el valor predeterminado de esta propiedad es verdadero. Si el usuario necesita mantener todos los estilos en el libro de trabajo para el html generado (como el escenario en el que el usuario necesita restaurar el libro de trabajo del html generado más adelante), establezca esta propiedad como falsa . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indica si se exporta todo el libro de trabajo a un archivo html. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Obtiene o establece el área de celda de exportación de la hoja de trabajo activa actual. Si establece este atributo, se omitirá el área de impresión de la hoja de trabajo activa actual. Solo se exportará el área especificada al guardar el archivo en html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es verdadero. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Indica si se exporta la coordenada de Excel de las celdas que no están en blanco al guardar el archivo en html. El valor predeterminado es falso. Si desea importar el html de salida a Excel, mantenga el valor predeterminado. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Indica la regla de exportación de datos de archivo html. El valor predeterminado es Todo. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Indica si se están exportando las propiedades del documento. El valor predeterminado es verdadero. Si desea importar el archivo html o mht para excel, mantenga el valor predeterminado. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Indica si se exportan encabezados adicionales cuando la longitud del texto es más larga que la columna de visualización máxima. El valor predeterminado es falso. Si desea importar el archivo html a Excel, mantenga el valor predeterminado. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Indica si se exporta la fórmula al guardar el archivo en html. El valor predeterminado es verdadero. Si desea importar el html de salida a Excel, mantenga el valor predeterminado. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Indica si se exportan secuencias de comandos de fotogramas y propiedades del documento. El valor predeterminado es verdadero. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Indicando si se están exportando las cuadrículas. El valor por defecto es falso. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Indica si se está exportando el contenido oculto de la hoja de cálculo. El valor predeterminado es verdadero. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Indica si se exportan encabezados de página. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Indica si se exportan encabezados de página. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Indica si solo se exporta el área de impresión a archivo html. El valor predeterminado es falso. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Indica si se exportan los encabezados de fila y columna de la hoja al guardar en archivos HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Indica si se exporta el estilo de borde similar cuando los navegadores no admiten el estilo de borde. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Indica si exportar la pestaña única cuando el archivo solo tiene una hoja de trabajo. El valor predeterminado es falso. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Indica si se están exportando las propiedades del libro de trabajo. El valor predeterminado es verdadero. Si desea importar el archivo html o mht para sobresalir, mantenga el valor predeterminado. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Indica si exportar la hoja de trabajo css por separado. El valor predeterminado es falso. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Indica si se están exportando las propiedades de la hoja de cálculo. El valor predeterminado es verdadero. Si desea importar el archivo html o mht para sobresalir, mantenga el valor predeterminado. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Obtiene o establece el IFilePathProvider para exportar la hoja de trabajo a html por separado. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardar esto en formato html, si HtmlHiddenColDisplayType es "Eliminar", la columna oculta no se mostraría, si el valor está "Oculto", la columna se ha emitido, pero estaba oculto, el valor predeterminado es "Oculto" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardar esto en formato html, si HtmlHiddenRowDisplayType es "Eliminar", la fila oculta no se mostraría, si el valor está "Oculto", la fila se ha emitido, pero estaba oculto, el valor predeterminado es "Oculto" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Indica si una cadena de celdas cruzadas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato html. archivos creados por Aspose.Cells y MS Excel. Pero el rendimiento para crear archivos html grandes, establecer el valor en Cruz sería varias veces más rápido que establecerlo en Predeterminado o Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Indicar si exportar aquellas formas no visibles |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Obtenga el objeto ImageOrPrintOptions antes de exportar |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Indica si se usa una unidad escalable para describir el ancho de la imagen cuando se usa una unidad escalable para describir el ancho de la columna. El valor predeterminado es verdadero. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Indica si se exportan archivos de imagen al directorio temporal. Solo para guardar en flujo html. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Indica si al exportar comentarios al guardar el archivo en html, el valor predeterminado es falso. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Indica si se usa el enlace de ruta completa en sheet00x.htm,filelist.xml y tabstrip.htm. El valor predeterminado es false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | Indica el tipo de atributo de destino en el enlace &lt;a&gt;, el valor predeterminado es HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Indica si se fusiona el elemento TD vacío a la fuerza al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente después de establecer el valor en verdadero. El valor predeterminado es falso. Si desea importar el archivo html para sobresalir o exportar líneas de cuadrícula perfectas al guardar el archivo en html, mantenga el valor predeterminado. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | El título de la página html. Solo para guardar en flujo html. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Analizar la etiqueta html en la celda, como ,como valor de celda o como etiqueta html, el valor predeterminado es true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es falso. Si desea obtener una presentación más hermosa, establezca el valor en verdadero. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica si se están actualizando los datos de la memoria caché del gráfico |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Indica si guardar el html como archivo único. El valor predeterminado es falso. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtiene el formato de archivo guardado. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Indica si mostrar todas las hojas al guardar como un solo archivo html. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica si ordenar los nombres definidos externos antes de guardar el archivo. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica si ordenar los nombres definidos antes de guardar el archivo. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Obtiene o establece el IStreamProvider para exportar objetos. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Obtiene y establece el prefijo del nombre de tipo css, como tr, col, td, etc., están contenidos en el elemento de tabla que tiene el atributo TableCssId específico. El valor predeterminado es "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica si se está actualizando la configuración de arte inteligente. El valor predeterminado es falso. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica si validar las celdas combinadas antes de guardar el archivo. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Indica si se utiliza una unidad escalable para describir el ancho de columna al exportar el archivo a html. El valor predeterminado es false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Indica si acercar o alejar el html a través del nivel de zoom de la hoja de trabajo al guardar el archivo en html, el valor predeterminado es falso. |

### Ver también

* class [SaveOptions](../saveoptions)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
