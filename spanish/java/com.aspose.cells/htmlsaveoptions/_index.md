---
title: "HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para guardar el archivo html."
type: docs
url: /es/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Representa las opciones para guardar el archivo html.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Crea opciones para guardar un archivo html. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | Crea opciones para guardar un archivo htm. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Indica si se debe agregar una fuente genérica a la propiedad CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | El directorio donde se guardarán los archivos adjuntos. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCalculateFormula()](#getCalculateFormula--) | Indica si se deben calcular las fórmulas antes de guardar el archivo html. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Obtiene el prefijo del nombre css, el valor predeterminado es "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Especifica el atributo que indica el CellName que se debe escribir. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getCssStyles()](#getCssStyles--) | Obtiene los estilos css adicionales para el formateador. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Representa el modo de renderizar DataBar al convertir archivos Excel a archivos html. |
| [getDefaultFontName()](#getDefaultFontName--) | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null. |
| [getDisableCss()](#getDisableCss--) | Indica si solo se aplican estilos en línea, sin depender de CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indica si se desactivan los comentarios condicionales Downlevel-revealed al exportar el archivo a html, el valor predeterminado es false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Obtiene el tipo de incrustación del archivo de fuente en el archivo html. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Optimiza la salida de html usando propiedades personalizadas de CSS. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Indica si las entidades de caracteres html se reemplazan con código decimal. |
| [getEncoding()](#getEncoding--) | Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indica si se excluyen los estilos no utilizados. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indica si solo se exporta la hoja de cálculo activa a un archivo html. |
| [getExportArea()](#getExportArea--) | Obtiene el CellArea de exportación de la hoja de cálculo activa actual. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Indica si se exportan datos falsos de la fila inferior. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. |
| [getExportCommentsType()](#getExportCommentsType--) | Representa el tipo de exportación de comentarios a archivos html. |
| [getExportDataOptions()](#getExportDataOptions--) | Indica la regla de exportación de datos del archivo html. El valor predeterminado es All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Indica si se exportan encabezados adicionales cuando la longitud del texto supera la columna de visualización máxima. |
| [getExportFormula()](#getExportFormula--) | Indica si se exporta la fórmula al guardar el archivo en html. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Indica si se exportan los scripts de marco y las propiedades del documento. |
| [getExportGridLines()](#getExportGridLines--) | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [getExportHeadings()](#getExportHeadings--) | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Indica si se exportan los elementos de anclaje para rangos con nombre al guardar como HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | Obtiene el ExportObjectListener para exportar objetos. |
| [getExportPageFooters()](#getExportPageFooters--) | Indica si se exportan los encabezados de página. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indica si se exportan los encabezados de página. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indica si solo se exporta el área de impresión al archivo html. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. |
| [getExportSingleTab()](#getExportSingleTab--) | Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [getFilePathProvider()](#getFilePathProvider--) | Obtiene el IFilePathProvider para exportar la hoja de cálculo a html por separado. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta, el valor predeterminado es "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se exportará; si el valor es "Hidden", la fila se exportará pero permanecerá oculta, el valor predeterminado es "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Indica si se oculta el texto desbordado cuando el formato de la celda está configurado para ajustar texto. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Indica si una cadena que abarca varias celdas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato html. |
| [getHtmlVersion()](#getHtmlVersion--) | Especifica la versión del estándar HTML que se debe usar al guardar en formato HTML. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Indica si se exportan las formas no visibles. |
| [getImageOptions()](#getImageOptions--) | Obtenga el objeto ImageOrPrintOptions antes de exportar. |
| [getImageScalable()](#getImageScalable--) | Indica si se utiliza una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. |
| [getLayoutMode()](#getLayoutMode--) | Obtiene el modo de diseño al guardar en HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | Indicando el tipo de atributo objetivo en el enlace `<a>`. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Indica si se fusiona obligatoriamente el elemento TD vacío al exportar el archivo a HTML. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image. |
| [getPageTitle()](#getPageTitle--) | El título de la página HTML. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Indica si la etiqueta HTML (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. |
| [getPresentationPreference()](#getPresentationPreference--) | Indicando si el archivo html o mht es la preferencia de presentación. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Indica si se guarda el HTML como un solo archivo. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSheetSet()](#getSheetSet--) | Obtiene las hojas a renderizar. |
| [getShowAllSheets()](#getShowAllSheets--) | Indica si se muestran todas las hojas al guardar como un único archivo HTML. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getSpaceMode()](#getSpaceMode--) | Indica cómo se renderizan los espacios en la salida HTML. |
| [getStreamProvider()](#getStreamProvider--) | Obtiene el IStreamProvider para exportar objetos. |
| [getTableCssId()](#getTableCssId--) | Obtiene el prefijo del nombre de tipo CSS como tr, col, td, etc., que están contenidos en el elemento tabla que tiene el atributo TableCssId específico. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [getWidthScalable()](#getWidthScalable--) | Indica si se exporta el ancho de columna en unidades de escala a HTML. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indica si se hace zoom in o out del HTML mediante el nivel de zoom de la hoja al guardar el archivo en HTML, el valor predeterminado es false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Indica si los bordes de la tabla están colapsados. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indica si se exportan los archivos de imagen al directorio temporal. |
| [isExportComments()](#isExportComments--) | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [isFullPathLink()](#isFullPathLink--) | Indicando si se utiliza enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Indicando si el HTML de salida es compatible con el navegador IE. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Indica si JavaScript es compatible con navegadores que no soportan JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Indica si el HTML de salida es compatible con dispositivos móviles. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Indica si se debe agregar una fuente genérica a la propiedad CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | El directorio donde se guardarán los archivos adjuntos. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Indica si los bordes de la tabla están colapsados. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica si se deben calcular las fórmulas antes de guardar el archivo html. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Establece el prefijo del nombre CSS, el valor predeterminado es "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Especifica el atributo que indica el CellName que se debe escribir. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Establece los estilos CSS adicionales para el formateador. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Representa el modo de renderizar DataBar al convertir archivos Excel a archivos html. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Indica si solo se aplican estilos en línea, sin depender de CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Indica si se desactivan los comentarios condicionales Downlevel-revealed al exportar el archivo a html, el valor predeterminado es false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Establece el tipo de incrustación del archivo de fuente en el archivo HTML. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Optimiza la salida de html usando propiedades personalizadas de CSS. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Indica si las entidades de caracteres html se reemplazan con código decimal. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Indica si se excluyen los estilos no utilizados. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Indica si se exportan los archivos de imagen al directorio temporal. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indica si solo se exporta la hoja de cálculo activa a un archivo html. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Establece el CellArea de exportación de la Worksheet activa actual. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Indica si se exportan datos falsos de la fila inferior. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Representa el tipo de exportación de comentarios a archivos html. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Indica la regla de exportación de datos del archivo html. El valor predeterminado es All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Indica si se exportan encabezados adicionales cuando la longitud del texto supera la columna de visualización máxima. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Indica si se exporta la fórmula al guardar el archivo en html. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Indica si se exportan los scripts de marco y las propiedades del documento. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Indica si se exportan los elementos de anclaje para rangos con nombre al guardar como HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Establece el ExportObjectListener para la exportación de objetos. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Indica si se exportan los encabezados de página. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Indica si se exportan los encabezados de página. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indica si solo se exporta el área de impresión al archivo html. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Establece el IFilePathProvider para exportar la Worksheet a HTML por separado. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indicando si se utiliza enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta, el valor predeterminado es "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se exportará; si el valor es "Hidden", la fila se exportará pero permanecerá oculta, el valor predeterminado es "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Indica si se oculta el texto desbordado cuando el formato de la celda está configurado para ajustar texto. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Indica si una cadena que abarca varias celdas se mostrará de la misma manera que MS Excel al guardar un archivo de Excel en formato html. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Especifica la versión del estándar HTML que se debe usar al guardar en formato HTML. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Indicando si el HTML de salida es compatible con el navegador IE. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Indica si se exportan las formas no visibles. |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Indica si se utiliza una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Indica si JavaScript es compatible con navegadores que no soportan JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Establece el modo de diseño al guardar en HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Indicando el tipo de atributo objetivo en el enlace `<a>`. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Indica si se fusiona obligatoriamente el elemento TD vacío al exportar el archivo a HTML. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Indica si el HTML de salida es compatible con dispositivos móviles. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | El título de la página HTML. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Indica si la etiqueta HTML (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indicando si el archivo html o mht es la preferencia de presentación. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Indica si se guarda el HTML como un solo archivo. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Establece las hojas a renderizar. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Indica si se muestran todas las hojas al guardar como un único archivo HTML. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Indica cómo se renderizan los espacios en la salida HTML. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Establece el IStreamProvider para exportar objetos. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Establece el prefijo del nombre css de tipo, como tr, col, td, etc., que se encuentran en el elemento table que tiene el atributo TableCssId específico. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Indica si se exporta el ancho de columna en unidades de escala a HTML. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Indica si se hace zoom in o out del HTML mediante el nivel de zoom de la hoja al guardar el archivo en HTML, el valor predeterminado es false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Crea opciones para guardar un archivo html.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


Crea opciones para guardar un archivo htm.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de archivo. Debe ser uno de los siguientes tipos: [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) o [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML), de lo contrario el formato guardado se establecerá automáticamente como [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


El directorio donde se guardarán los archivos adjuntos. Solo para guardar en un flujo HTML.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Especifique el prefijo Url de los archivos adjuntos, como imágenes en el archivo HTML. Solo para guardar en un flujo HTML.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La carpeta para archivos temporales que pueden usarse como caché de datos.

**Remarks**

Si no se ha especificado la carpeta, el valor predeterminado es [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si su valor predeterminado es nulo o está vacío, o se ha especificado como nulo o vacío, entonces no se utilizará ningún archivo de caché al guardar el libro de trabajo.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica si se deben calcular las fórmulas antes de guardar el archivo html.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Obtiene el prefijo del nombre css, el valor predeterminado es "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Especifica el atributo que indica el CellName a escribir. (p. ej., si el valor es \"id\", entonces para la celda \"A1\", la salida será: <td id='A1'>). El valor predeterminado es null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando ingresa un valor más largo que 32K, se truncará.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Deja el libro de trabajo vacío después de guardar el archivo.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Obtiene los estilos css adicionales para el formateador. Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True. CssStyles=\"body \{ padding: 5px \}\";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Representa el modo de renderizado de DataBar al convertir archivos Excel a archivos HTML. El valor predeterminado es [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Ver [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Indica si solo se aplican estilos en línea, sin depender de CSS. El valor predeterminado es false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Indica si se desactivan los comentarios condicionales Downlevel-revealed al exportar el archivo a html, el valor predeterminado es false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Obtiene el tipo de incrustación de archivo de fuente en el archivo HTML. El valor predeterminado es [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE), lo que indica que no se incrustará ninguna fuente en HTML.

Ver [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Optimiza la salida de HTML usando propiedades personalizadas de CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64, con una propiedad personalizada los datos de la imagen solo necesitan guardarse una vez, lo que mejora el rendimiento del HTML resultante. El valor predeterminado es false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Indica si las entidades de caracteres HTML se reemplazan con código decimal. (p. ej., \"&nbsp;\" se reemplaza con \"&\#160;\"). El valor predeterminado es false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true.

**Remarks**

Solo para archivos .xls, .xlsx, .xlsb y .xlsm.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Indica si se excluyen los estilos no utilizados. Para los archivos HTML generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita conservar todos los estilos en el libro de trabajo para el HTML generado (por ejemplo, en el caso de que necesite restaurar el libro de trabajo a partir del HTML generado más tarde), establezca esta propiedad como false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indica si solo se exporta la Worksheet activa a un archivo HTML. Si es true, solo la Worksheet activa se exportará al archivo HTML; si es false, todo el libro de trabajo se exportará al archivo HTML. El valor predeterminado es false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Obtiene el CellArea de exportación de la Worksheet activa actual. Si establece este atributo, el área de impresión de la Worksheet activa se omitirá. Solo el área especificada se exportará al guardar el archivo en HTML.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si desea importar el archivo HTML o MHT a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Representa el tipo de exportación de comentarios a archivos html.

Ver [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Indica la regla de exportación de datos del archivo html. El valor predeterminado es All.

Ver [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Indica si se exportan encabezados adicionales cuando la longitud del texto es mayor que la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Indica si se exportan scripts de marco y propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad HtmlSaveOptions.ExportRowColumnHeadings. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB.

**Remarks**

Cuando esta propiedad se establece en true, los datos de la imagen se exportan directamente en los elementos img y no se crean archivos separados.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Indica si se exportan elementos de anclaje para rangos con nombre al guardar como HTML. El valor predeterminado es true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Obtiene el ExportObjectListener para exportar objetos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad HtmlSaveOptions.IStreamProvider. Esta propiedad será eliminada 12 meses después, a partir de agosto de 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Indica si se exportan los encabezados de página.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Indica si se exportan los encabezados de página.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Obtiene el IFilePathProvider para exportar la hoja de cálculo a html por separado.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true, se ignora el ancho de la columna y se exportará todo el dato de la celda. Si es false, los datos se exportarán igual que en Excel. El valor predeterminado es false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta, el valor predeterminado es "Hidden".

Ver [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se exportará; si el valor es "Hidden", la fila se exportará pero permanecerá oculta, el valor predeterminado es "Hidden".

Ver [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Indica si se oculta el texto desbordado cuando el formato de la celda está configurado para ajustar texto. El valor predeterminado es false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Indica si una cadena que cruza celdas se mostrará de la misma forma que MS Excel al guardar un archivo Excel en formato html. Por defecto el valor es Default, por lo que, para cadenas que cruzan celdas, hay poca diferencia entre los archivos html creados por Aspose.Cells y MS Excel. Pero el rendimiento al crear archivos html grandes, establecer el valor en Cross sería varias veces más rápido que establecerlo en Default o Fit2Cell.

Ver [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Especifica la versión del estándar HTML que debe usarse al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default.

Ver [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Indica si se exportan las formas no visibles.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Obtenga el objeto ImageOrPrintOptions antes de exportar.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Indica si se usa una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. El valor predeterminado es true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Obtiene el modo de diseño al guardar en HTML. El valor predeterminado es [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Ver [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Indica el tipo del atributo target en el enlace `<a>`. El valor predeterminado es HtmlLinkTargetType.Parent.

Ver [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Indica si se fusiona obligatoriamente el elemento TD vacío al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente al establecer el valor en true. El valor predeterminado es false. Si desea importar el archivo html a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, mantenga el valor predeterminado.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default.

Ver [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image.

Ver [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


El título de la página html. Solo para guardar en un flujo html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Indica si la etiqueta html (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica si se almacena en caché los datos más recientes del gráfico.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Indica si se guarda el html como un solo archivo. El valor predeterminado es false.

**Remarks**

Si hay varias hojas de cálculo u otros recursos necesarios, como imágenes, en el libro, normalmente esas hojas y recursos deben guardarse en archivos separados. En algunos escenarios, el usuario puede necesitar obtener un solo archivo resultante para facilitar la transferencia. En ese caso, el usuario puede establecer esta propiedad en true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el formato de archivo guardado.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtiene las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Indica si se muestran todas las hojas al guardar como un único archivo HTML.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indica si se ordenan los nombres definidos externos antes de guardar el archivo.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica si se ordenan los nombres definidos antes de guardar el archivo.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Indica cómo se renderizan los espacios en la salida HTML. Esta opción se aplica actualmente solo a formatos numéricos (p. ej., formato contable). El valor predeterminado es [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Ver [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtiene el IStreamProvider para exportar objetos.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Obtiene el prefijo del nombre CSS de tipo, como tr, col, td, etc., que están contenidos en el elemento tabla que tiene el atributo TableCssId específico. El valor predeterminado es "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica si se actualiza la configuración de SmartArt. El valor predeterminado es false.

**Remarks**

Solo tiene efecto después de llamar al método Shape.GetResultOfSmartArt() y cuando las formas en caché existen en el archivo de plantilla.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indica si se validan las celdas combinadas antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtiene la devolución de llamada de advertencia.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Indica si se exporta el ancho de columna en unidades de escala a html. El valor predeterminado es false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Indica si se hace zoom in o out del HTML mediante el nivel de zoom de la hoja al guardar el archivo en HTML, el valor predeterminado es false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


Indica si los bordes de la tabla están colapsados. El valor predeterminado es true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Indica si se exportan los archivos de imagen a un directorio temporal. Solo para guardar en un flujo html.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indica si se utiliza un enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


Indica si se debe agregar una fuente genérica a la familia de fuentes CSS. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


El directorio donde se guardarán los archivos adjuntos. Solo para guardar en un flujo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Especifique el prefijo Url de los archivos adjuntos, como imágenes en el archivo HTML. Solo para guardar en un flujo HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Indica si los bordes de la tabla están colapsados. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La carpeta para archivos temporales que pueden usarse como caché de datos.

**Remarks**

Si no se ha especificado la carpeta, el valor predeterminado es [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si su valor predeterminado es nulo o está vacío, o se ha especificado como nulo o vacío, entonces no se utilizará ningún archivo de caché al guardar el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica si se deben calcular las fórmulas antes de guardar el archivo html.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Establece el prefijo del nombre CSS, el valor predeterminado es "".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Especifica el atributo que indica el CellName a escribir. (p. ej., si el valor es \"id\", entonces para la celda \"A1\", la salida será: <td id='A1'>). El valor predeterminado es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando ingresa un valor más largo que 32K, se truncará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Deja el libro de trabajo vacío después de guardar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Establece los estilos CSS adicionales para el formateador. Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.  CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Representa el modo de renderizado de DataBar al convertir archivos Excel a archivos HTML. El valor predeterminado es [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Ver [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Indica si solo se aplican estilos en línea, sin depender de CSS. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Indica si se desactivan los comentarios condicionales Downlevel-revealed al exportar el archivo a html, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Establece el tipo de incrustación del archivo de fuente en el archivo html. El valor predeterminado es [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) que indica que no se incrustará ninguna fuente en html.

Ver [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Optimiza la salida de HTML usando propiedades personalizadas de CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64, con una propiedad personalizada los datos de la imagen solo necesitan guardarse una vez, lo que mejora el rendimiento del HTML resultante. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Indica si las entidades de caracteres HTML se reemplazan con código decimal. (p. ej., \"&nbsp;\" se reemplaza con \"&\#160;\"). El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true.

**Remarks**

Solo para archivos .xls, .xlsx, .xlsb y .xlsm.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Indica si se excluyen los estilos no utilizados. Para los archivos HTML generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita conservar todos los estilos en el libro de trabajo para el HTML generado (por ejemplo, en el caso de que necesite restaurar el libro de trabajo a partir del HTML generado más tarde), establezca esta propiedad como false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Indica si se exportan los archivos de imagen a un directorio temporal. Solo para guardar en un flujo html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indica si solo se exporta la Worksheet activa a un archivo HTML. Si es true, solo la Worksheet activa se exportará al archivo HTML; si es false, todo el libro de trabajo se exportará al archivo HTML. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Establece el área de celda a exportar de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si desea importar el archivo HTML o MHT a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Indica si se exportan las coordenadas de Excel de las celdas no vacías al guardar el archivo en html. El valor predeterminado es false. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Representa el tipo de exportación de comentarios a archivos html.

Ver [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Indica la regla de exportación de datos del archivo html. El valor predeterminado es All.

Ver [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Indica si se exportan encabezados adicionales cuando la longitud del texto es mayor que la columna de visualización máxima. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Indica si se exportan fórmulas al guardar el archivo en html. El valor predeterminado es true. Si desea importar el html generado a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Indica si se exportan scripts de marco y propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad HtmlSaveOptions.ExportRowColumnHeadings. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB.

**Remarks**

Cuando esta propiedad se establece en true, los datos de la imagen se exportan directamente en los elementos img y no se crean archivos separados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Indica si se exportan elementos de anclaje para rangos con nombre al guardar como HTML. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Establece el ExportObjectListener para la exportación de objetos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad HtmlSaveOptions.IStreamProvider. Esta propiedad será eliminada 12 meses después, a partir de agosto de 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Indica si se exportan los encabezados de página.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Indica si se exportan los encabezados de página.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Indica si se exporta un estilo de borde similar cuando el estilo de borde no es compatible con los navegadores. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Indica si se exporta el CSS de la hoja de cálculo por separado. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Indica si se exportan las propiedades de la hoja de cálculo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Establece el IFilePathProvider para exportar la Worksheet a HTML por separado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Indica si se muestra todo el dato formateado de la celda cuando desborda la columna. Si es true, se ignora el ancho de la columna y se exportará todo el dato de la celda. Si es false, los datos se exportarán igual que en Excel. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indica si se utiliza un enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Columna oculta (el ancho de esta columna es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenColDisplayType es "Remove", la columna oculta no se exportará; si el valor es "Hidden", la columna se exportará pero permanecerá oculta, el valor predeterminado es "Hidden".

Ver [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Fila oculta (la altura de esta fila es 0) en Excel, antes de guardarla en formato html, si HtmlHiddenRowDisplayType es "Remove", la fila oculta no se exportará; si el valor es "Hidden", la fila se exportará pero permanecerá oculta, el valor predeterminado es "Hidden".

Ver [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Indica si se oculta el texto desbordado cuando el formato de la celda está configurado para ajustar texto. El valor predeterminado es false

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Indica si una cadena que cruza celdas se mostrará de la misma forma que MS Excel al guardar un archivo Excel en formato html. Por defecto el valor es Default, por lo que, para cadenas que cruzan celdas, hay poca diferencia entre los archivos html creados por Aspose.Cells y MS Excel. Pero el rendimiento al crear archivos html grandes, establecer el valor en Cross sería varias veces más rápido que establecerlo en Default o Fit2Cell.

Ver [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Especifica la versión del estándar HTML que debe usarse al guardar en formato HTML. El valor predeterminado es HtmlVersion.Default.

Ver [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Indica si el HTML de salida es compatible con el navegador IE. El valor predeterminado es false

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Indica si se exportan las formas no visibles.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Indica si se usa una unidad escalable para describir el ancho de la imagen al usar una unidad escalable para describir el ancho de la columna. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Indica si JavaScript es compatible con navegadores que no soportan JavaScript. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Establece el modo de diseño al guardar en HTML. El valor predeterminado es [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Ver [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Indica el tipo del atributo target en el enlace `<a>`. El valor predeterminado es HtmlLinkTargetType.Parent.

Ver [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Indica si se fusiona obligatoriamente el elemento TD vacío al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente al establecer el valor en true. El valor predeterminado es false. Si desea importar el archivo html a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, mantenga el valor predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default.

Ver [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Indica cómo se exportan los objetos OfficeMath a HTML, el valor predeterminado es Image.

Ver [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


El título de la página html. Solo para guardar en un flujo html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Indica si la etiqueta html (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica si se almacena en caché los datos más recientes del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Indica si se guarda el html como un solo archivo. El valor predeterminado es false.

**Remarks**

Si hay varias hojas de cálculo u otros recursos necesarios, como imágenes, en el libro, normalmente esas hojas y recursos deben guardarse en archivos separados. En algunos escenarios, el usuario puede necesitar obtener un solo archivo resultante para facilitar la transferencia. En ese caso, el usuario puede establecer esta propiedad en true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Establece las hojas a renderizar. El predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Indica si se muestran todas las hojas al guardar como un único archivo HTML.

**Remarks**

Solo funciona cuando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) es True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indica si se ordenan los nombres definidos externos antes de guardar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indica si se ordenan los nombres definidos antes de guardar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Indica cómo se renderizan los espacios en la salida HTML. Esta opción se aplica actualmente solo a formatos numéricos (p. ej., formato contable). El valor predeterminado es [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Ver [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Establece el IStreamProvider para exportar objetos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Establece el prefijo del nombre CSS de tipo, como tr, col, td, etc., que se encuentran en el elemento table que tiene el atributo TableCssId específico. El valor predeterminado es "".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indica si se actualiza la configuración de SmartArt. El valor predeterminado es false.

**Remarks**

Solo tiene efecto después de llamar al método Shape.GetResultOfSmartArt() y cuando las formas en caché existen en el archivo de plantilla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indica si se validan las celdas combinadas antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Establece la devolución de llamada de advertencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Indica si se exporta el ancho de columna en unidades de escala a html. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Indica si se hace zoom in o out del HTML mediante el nivel de zoom de la hoja al guardar el archivo en HTML, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

