---
title: "Clase EbookSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Saving.EbookSaveOptions clase. Representa las opciones para guardar un archivo ebook."
type: docs
url: /es/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Representa las opciones para guardar el archivo ebook.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Crea opciones para guardar el archivo ebook. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Crea opciones para guardar el archivo ebook. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | El directorio donde se guardarán los archivos adjuntos. Solo para guardar en flujo html. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. Solo para guardar en flujo html. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indica si se deben calcular las fórmulas antes de guardar el archivo html. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Obtiene y establece el prefijo del nombre css, el valor predeterminado es "". (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Especifica el atributo que indica el CellName a escribir. (p. ej., si el valor es "id", entonces para la celda "A1", la salida será:&lt;td id='A1'&gt;). El valor predeterminado es null. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, excel no permite ingresar un valor de cadena mayor a 32K. Cuando se ingresa un valor mayor a 32K, se truncará. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Deja el libro de trabajo vacío después de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es true y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Obtiene o establece los estilos css adicionales para el formateador. Solo funciona cuando [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) es True. CssStyles="body { padding: 5px }"; (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Representa el modo de renderizar DataBar al convertir archivos Excel a archivos html. El valor predeterminado es BackgroundColor. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Especifique el nombre de fuente predeterminado para exportar html, la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es null, Aspose.Cells usará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indica si solo se aplican estilos en línea, sin depender de CSS. El valor predeterminado es false. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indica si se deshabilitan los comentarios condicionales revelados de nivel inferior al exportar el archivo a html, el valor predeterminado es false. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Obtiene o establece el tipo de incrustación de archivo de fuente en el archivo html. El valor predeterminado es None, lo que indica que no se incrustará ninguna fuente en html. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimiza la salida de html usando propiedades personalizadas de CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64, con una propiedad personalizada los datos de la imagen solo necesitan guardarse una vez, por lo que el rendimiento del html resultante puede mejorarse. El valor predeterminado es false. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indica si las entidades de caracteres html se reemplazan con código decimal. (p. ej., "&amp;nbsp;" se reemplaza con "&amp;#160;"). El valor predeterminado es false. (Hereditado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Si no se establece, use Encoding.UTF8 como tipo de codificación predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true. (Heredado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indica si se excluyen los estilos no utilizados. Para los archivos html generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita mantener todos los estilos en el libro de trabajo para el html generado (por ejemplo, el escenario en que el usuario necesita restaurar el libro de trabajo desde el html generado más tarde), establezca esta propiedad como false. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica si solo se exporta la hoja de cálculo activa a un archivo html. Si es true, solo la hoja activa se exportará al archivo html; si es false, todo el libro de trabajo se exportará al archivo html. El valor predeterminado es false. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Obtiene o establece la exportación del CellArea de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en html. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html generado a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Representa el tipo de exportación de comentarios a archivos html. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indica la regla de exportación de datos del archivo html. El valor predeterminado es All. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indica si se exportan encabezados extra cuando la longitud del texto supera la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si desea importar el html generado a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indica si se exportan scripts de marco y propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica si se exporta el contenido de la hoja de cálculo oculta. El valor predeterminado es true. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indica si se exportan los elementos de anclaje para rangos con nombre al guardar como HTML. El valor predeterminado es true. (Heredado de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsoleto.**) Obtiene o establece el ExportObjectListener para exportar objetos.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indica si se exportan los encabezados de página.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indica si se exportan los encabezados de página.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indica si solo se exporta el área de impresión a un archivo html. El valor predeterminado es false.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. El valor predeterminado es false.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Obtiene o establece el IFilePathProvider para exportar la hoja de cálculo a html por separado.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true entonces se ignora el ancho de columna y se exportará todo el dato de la celda. Si es false entonces el dato se exportará igual que en Excel. El valor predeterminado es false.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se emitirá; si el valor es "Hidden", la columna se emitirá, pero permanecerá oculta. El valor predeterminado es "Hidden"(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se emitirá; si el valor es "Hidden", la fila se emitirá, pero permanecerá oculta. El valor predeterminado es "Hidden"(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indica si se oculta el texto desbordado cuando el formato de la celda está configurado para ajustar texto. El valor predeterminado es false(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indica si una cadena que abarca varias celdas se mostrará de la misma manera que MS Excel al guardar un archivo Excel en formato html. Por defecto el valor es Default, por lo que, para cadenas que abarcan varias celdas, hay poca diferencia entre los archivos html creados por Aspose.Cells y MS Excel. Pero el rendimiento al crear archivos html grandes, al establecer el valor en Cross sería varias veces más rápido que establecerlo en Default o Fit2Cell.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Especifica la versión del estándar HTML que se debe usar al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default.(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indica si se exportan las formas no visibles(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Obtenga el objeto ImageOrPrintOptions antes de exportar(Her...`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indica si se usa unidad escalable para describir el ancho de la imagen al usar unidad escalable para describir el ancho de la columna. El valor predeterminado es true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indica si los bordes de la tabla están colapsados. El valor predeterminado es true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indica si se exportan archivos de imagen al directorio temporal. Solo para guardar en flujo html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indica si se exportan los comentarios al guardar el archivo en html, el valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indica si se usa enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Obtiene o establece el modo de diseño al guardar en HTML. El valor predeterminado es Normal(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indica el tipo de atributo target en el enlace `<a>`. El valor predeterminado es HtmlLinkTargetType.Parent.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsoleto.**) Indica si se fusionan forzosamente los elementos TD vacíos al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente después de establecer el valor a true. El valor predeterminado es false. Si desea importar el archivo html a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, mantenga el valor predeterminado.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indica cómo se exportan los objetos OfficeMath a HTML. El valor predeterminado es Image.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | El título de la página html. Solo para guardar en flujo html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indica si la etiqueta html (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor a true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indica si se guarda el html como un solo archivo. El valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indica si se muestran todas las hojas al guardar como un solo archivo html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indica cómo se representan los espacios en la salida HTML. Esta opción se aplica actualmente solo a formatos numéricos (p. ej., formato contable). El valor predeterminado es Css.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Obtiene o establece el IStreamProvider para exportar objetos.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Obtiene y establece el prefijo del nombre css del tipo, como tr, col, td, etc., que se encuentran en el elemento table que tiene el atributo TableCssId específico. El valor predeterminado es "".(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de smart art. El valor predeterminado es false.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indica si se exporta el ancho de columna en unidades de escala a html. El valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indica si se hace zoom in o zoom out del html mediante el nivel de zoom de la hoja de cálculo al guardar el archivo a html, el valor predeterminado es false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Crea una instancia de EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Estableciendo propiedades
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Guarda el libro de trabajo en un archivo HTML con las opciones especificadas
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


