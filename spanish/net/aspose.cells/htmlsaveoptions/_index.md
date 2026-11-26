---
title: "Clase HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HtmlSaveOptions. Representa las opciones para guardar un archivo html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Representa las opciones para guardar un archivo html.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Crea opciones para guardar un archivo html. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Crea opciones para guardar un archivo htm. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | El directorio donde se guardarán los archivos adjuntos. Solo para guardar en un flujo html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. Solo para guardar en un flujo html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indica si se deben calcular las fórmulas antes de guardar el archivo html. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Obtiene y establece el prefijo del nombre css, el valor predeterminado es "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Especifica el atributo que indica el CellName a escribir. (p.ej., si el valor es "id", entonces para la celda "A1", la salida será:&lt;td id='A1'&gt;). El valor predeterminado es null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Obtiene o establece los estilos css adicionales para el formateador. Solo funciona cuando [`SaveAsSingleFile`](./saveassinglefile/) es True. CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Representa el modo de renderizado de DataBar al convertir archivos Excel a archivos html. El valor predeterminado es BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es null, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original. El valor predeterminado es null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indica si solo se aplican estilos en línea, sin depender de CSS. El valor predeterminado es false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indica si se deshabilitan los comentarios condicionales revelados de nivel inferior al exportar el archivo a html, el valor predeterminado es false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Obtiene o establece el tipo de incrustación de archivos de fuente en el archivo html. El valor predeterminado es None, lo que indica que no se incrustará ninguna fuente en html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimiza la salida de html usando propiedades personalizadas de CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64, con una propiedad personalizada los datos de la imagen solo necesitan guardarse una vez, lo que mejora el rendimiento del html resultante. El valor predeterminado es false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indica si las entidades de caracteres html se reemplazan con código decimal. (p.ej., "&amp;nbsp;" se reemplaza con "&amp;#160;"). El valor predeterminado es false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Si no se establece, use Encoding.UTF8 como tipo de codificación predeterminado. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indica si se excluyen los estilos no utilizados. Para los archivos html generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita mantener todos los estilos en el libro de trabajo para el html generado (por ejemplo, si necesita restaurar el libro de trabajo a partir del html generado más tarde), establezca esta propiedad como false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica si solo se exporta la hoja de cálculo activa a un archivo html. Si es true, solo la hoja activa se exportará a html; si es false, todo el libro de trabajo se exportará a html. El valor predeterminado es false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Obtiene o establece el CellArea de exportación de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html generado a Excel, mantenga el valor predeterminado. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Representa el tipo de exportación de comentarios a archivos html. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indica la regla de exportación de datos del archivo html. El valor predeterminado es All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indica si se exportan encabezados adicionales cuando la longitud del texto supera la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si desea importar el html generado a Excel, mantenga el valor predeterminado. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indica si se exportan scripts de marco y propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indica si se exportan los elementos de anclaje para rangos con nombre al guardar como HTML. El valor predeterminado es true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Obtiene o establece el ExportObjectListener para exportar objetos. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indica si se exportan los encabezados de página. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indica si se exportan los encabezados de página. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Obtiene o establece el IFilePathProvider para exportar la hoja de cálculo a html por separado. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true, se ignora el ancho de columna y se exportará todo el dato de la celda. Si es false, el dato se exportará igual que en Excel. El valor predeterminado es false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta. El valor predeterminado es "Hidden". |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato HTML, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se generará, si el valor es "Hidden", la fila se generará pero permanecerá oculta, el valor predeterminado es "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indica si se debe ocultar el texto que se desborda cuando el formato de la celda está configurado para ajustar texto. El valor predeterminado es false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indica si una cadena que abarca varias celdas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato HTML. Por defecto el valor es Default, por lo que, para cadenas que cruzan celdas, hay poca diferencia entre los archivos HTML creados por Aspose.Cells y MS Excel. Sin embargo, el rendimiento al crear archivos HTML grandes, al establecer el valor en Cross sería varias veces más rápido que establecerlo en Default o Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Especifica la versión del estándar HTML que debe usarse al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indica si se exportan las formas que no son visibles |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Obtenga el objeto ImageOrPrintOptions antes de exportar |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indica si se utiliza una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. El valor predeterminado es true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indica si los bordes de la tabla están colapsados. El valor predeterminado es true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indica si se exportan los archivos de imagen a un directorio temporal. Solo para guardar en flujo HTML. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indica si se utiliza una ruta completa en los enlaces de sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Obtiene o establece el modo de diseño al guardar en HTML. El valor predeterminado es Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indica el tipo del atributo target en el enlace `<a>`. El valor predeterminado es HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indica si se fusionan los elementos TD vacíos de forma forzada al exportar el archivo a HTML. El tamaño del archivo HTML se reducirá significativamente después de establecer el valor en true. El valor predeterminado es false. Si desea importar el archivo HTML a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en HTML, mantenga el valor predeterminado. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | El título de la página HTML. Solo para guardar en flujo HTML. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indica si la etiqueta HTML (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indica si se guarda el HTML como un solo archivo. El valor predeterminado es false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. Por defecto son todas las hojas visibles en el libro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indica si se muestran todas las hojas al guardar como un único archivo HTML. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indica cómo se renderizan los espacios en la salida HTML. Esta opción se aplica actualmente solo a formatos numéricos (p. ej., formato contable). El valor predeterminado es Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Obtiene o establece el IStreamProvider para exportar objetos. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Obtiene y establece el prefijo del nombre CSS del tipo, como tr, col, td, etc., que están contenidos en el elemento table que tiene el atributo TableCssId específico. El valor predeterminado es "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indica si se exporta el ancho de columna en unidades de escala a HTML. El valor predeterminado es false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indica si se aplica zoom al HTML mediante el nivel de zoom de la hoja de cálculo al guardar el archivo como HTML, el valor predeterminado es false. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea una instancia de HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Guarda el libro de trabajo como HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


