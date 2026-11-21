---
title: "PdfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para guardar un archivo pdf."
type: docs
url: /es/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

Representa las opciones para guardar un archivo pdf.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Crea las opciones para guardar un archivo PDF. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [getBookmark()](#getBookmark--) | Obtiene el objeto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCalculateFormula()](#getCalculateFormula--) | Indica si se deben calcular las fórmulas antes de guardar el archivo pdf. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCompliance()](#getCompliance--) | Obtiene el nivel de cumplimiento de los estándares PDF para los documentos de salida. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getCreatedTime()](#getCreatedTime--) | Obtiene la hora de generación del documento pdf. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Obtiene un valor que determina la forma en que [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) se exporta al archivo PDF. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtiene configuraciones personalizadas durante el renderizado. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtiene el idioma de edición predeterminado. |
| [getDefaultFont()](#getDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Indica si la barra de título de la ventana debe mostrar el título del documento. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Indica si se debe incrustar el adjunto para objetos Ole en Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True para incrustar fuentes TrueType. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Configuración para renderizar un metafichero Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Indica si se debe exportar la estructura del documento. |
| [getFontEncoding()](#getFontEncoding--) | Obtiene la codificación de fuentes incrustadas en pdf. |
| [getGridlineColor()](#getGridlineColor--) | Obtiene el color de la línea de cuadrícula. |
| [getGridlineType()](#getGridlineType--) | Obtiene el tipo de línea de cuadrícula. |
| [getIgnoreError()](#getIgnoreError--) | Indica si necesita ocultar el error durante el renderizado. |
| [getImageType()](#getImageType--) | Representa el tipo de imagen al convertir el gráfico y la forma. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [getOptimizationType()](#getOptimizationType--) | Obtiene el tipo de optimización pdf. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [getPageCount()](#getPageCount--) | Obtiene el número de páginas a guardar. |
| [getPageIndex()](#getPageIndex--) | Obtiene el índice basado en cero de la primera página a guardar. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controla/Indica el progreso del proceso de guardado de página. |
| [getPdfCompression()](#getPdfCompression--) | Indica el algoritmo de compresión |
| [getPrintingPageType()](#getPrintingPageType--) | Indica qué páginas no se imprimirán. |
| [getProducer()](#getProducer--) | Obtiene el productor del documento pdf generado. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Obtiene los comportamientos de renderizado específicos de Excel a aplicar. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSecurityOptions()](#getSecurityOptions--) | Establezca estas opciones, cuando se necesite seguridad en el resultado xls2pdf. |
| [getSheetSet()](#getSheetSet--) | Obtiene las hojas a renderizar. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getTextCrossType()](#getTextCrossType--) | Obtiene el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [getWatermark()](#getWatermark--) | Obtiene la marca de agua para la salida. |
| [getZoomBehavior()](#getZoomBehavior--) | Obtiene el modo de vista inicial cuando se abre el documento PDF generado. |
| [getZoomFactor()](#getZoomFactor--) | Obtiene el porcentaje de zoom usado cuando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) es [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Establece el objeto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica si se deben calcular las fórmulas antes de guardar el archivo pdf. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCompliance(int value)](#setCompliance-int-) | Establece el nivel de cumplimiento de los estándares PDF para los documentos de salida. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Establece la hora de generación del documento pdf. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Establece un valor que determina la forma en que [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) se exporta al archivo PDF. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Establece configuraciones personalizadas durante la renderización. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Establece el idioma de edición predeterminado. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Indica si la barra de título de la ventana debe mostrar el título del documento. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Indica si se debe incrustar el adjunto para objetos Ole en Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | True para incrustar fuentes TrueType. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Configuración para renderizar un metafichero Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Indica si se debe exportar la estructura del documento. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Establece la codificación de fuentes incrustadas en pdf. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Establece el color de la línea de cuadrícula. |
| [setGridlineType(int value)](#setGridlineType-int-) | Establece el tipo de línea de cuadrícula. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica si necesita ocultar el error durante el renderizado. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Establece el PPI (píxeles por pulgada) deseado de las imágenes remuestreadas y la calidad JPEG. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Representa el tipo de imagen al convertir el gráfico y la forma. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Establece el tipo de optimización pdf. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [setPageCount(int value)](#setPageCount-int-) | Establece el número de páginas a guardar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Establece el índice basado en cero de la primera página a guardar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controla/Indica el progreso del proceso de guardado de página. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Indica el algoritmo de compresión |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indica qué páginas no se imprimirán. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Establece el productor del documento pdf generado. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Establece los comportamientos de renderizado específicos de Excel a aplicar. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Establezca estas opciones, cuando se necesite seguridad en el resultado xls2pdf. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Establece las hojas a renderizar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Establece el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Establece la marca de agua en la salida. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Establece el modo de vista inicial cuando se abre el documento PDF generado. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Establece el porcentaje de zoom usado cuando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) es [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Crea las opciones para guardar un archivo PDF.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto.

**Returns:**
boolean
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


Obtiene el objeto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
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


Indica si se deben calcular las fórmulas antes de guardar el archivo pdf.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando ingresa un valor más largo que 32K, se truncará.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto.

**Remarks**

El valor predeterminado es verdadero. Desactivar esta propiedad puede ofrecer mejor rendimiento. Pero cuando la fuente predeterminada o especificada del texto/carácter no puede usarse para renderizarlo, pueden aparecer caracteres ilegibles (como bloques) en el PDF generado. En tal situación el usuario debe mantener esta propiedad como verdadera para que se busque y use una fuente alternativa para renderizar el texto.

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar primero estos caracteres.

**Remarks**

El valor predeterminado es verdadero.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Obtiene el nivel de cumplimiento de los estándares PDF para los documentos de salida.

Ver [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

El valor predeterminado es Pdf17.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Obtiene la hora de generación del documento pdf.

**Remarks**

Si no se establece, será la hora de generar el PDF.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


Obtiene un valor que determina la forma en que [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) se exporta al archivo PDF. El valor predeterminado es None.

Ver [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Obtiene configuraciones personalizadas durante el renderizado.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Obtiene el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, establezca la DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

**Returns:**
java.lang.String
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Indica si la barra de título de la ventana debe mostrar el título del documento.

**Remarks**

Si es false, la barra de título debe mostrar en su lugar el nombre del archivo PDF. El valor predeterminado es false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Indica si se debe incrustar el adjunto para objetos Ole en Excel.

**Remarks**

El valor predeterminado es false. El valor debe ser false cuando se establece la conformidad PDF/A o el cifrado PDF está habilitado.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True para incrustar fuentes TrueType. Afecta solo a los caracteres ASCII 32-127. Las fuentes para códigos de caracteres mayores a 127 siempre se incrustan. Las fuentes siempre se incrustan para el estándar PDF/A-1a, PDF/A-1b. El valor predeterminado es true.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Configuración para renderizar un metafichero Emf.

Ver [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando se establece [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), los registros EMF+ se analizarán al renderizar la página; de lo contrario solo se analizarán los registros EMF. El valor predeterminado es [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true.

**Remarks**

Solo para archivos .xls, .xlsx, .xlsb y .xlsm.

**Returns:**
boolean
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Indica si se debe exportar la estructura del documento.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


Obtiene la codificación de fuentes incrustadas en pdf.

Ver [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

El valor predeterminado es [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtiene el color de la línea de cuadrícula.

**Remarks**

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Obtiene el tipo de línea de cuadrícula.

Ver [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

El valor predeterminado es tipo punteado.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indica si necesita ocultar el error durante la renderización. El error puede ser en forma, imagen, renderizado de gráfico, etc.

**Returns:**
boolean
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Representa el tipo de imagen al convertir el gráfico y la forma.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad del renderizado. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán aplicándose.

**Returns:**
boolean
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


Obtiene el tipo de optimización pdf.

Ver [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

El valor predeterminado es [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

**Remarks**

El valor predeterminado es verdadero.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtiene el número de páginas a guardar.

**Remarks**

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas.

**Example**

El siguiente ejemplo muestra cómo renderizar un rango de páginas (3 y 4) en un archivo Microsoft Excel a PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtiene el índice basado en cero de la primera página a guardar.

**Remarks**

El valor predeterminado es 0.

**Example**

El siguiente ejemplo muestra cómo renderizar un rango de páginas (3 y 4) en un archivo Microsoft Excel a PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Controla/Indica el progreso del proceso de guardado de página.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Indica el algoritmo de compresión

Ver [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Indica qué páginas no se imprimirán.

Ver [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Si el contenido de la hoja es escaso, algunas páginas pueden quedar totalmente en blanco en el archivo PDF de salida. Si no deseas esas páginas en blanco, puedes usar esta opción para omitirlas.

**Example**

El siguiente código omite páginas en blanco o páginas que solo contienen contenido de estilo, como fondo de celda y bordes.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getProducer() {#getProducer--}
```
public String getProducer()
```


Obtiene el productor del documento pdf generado.

**Remarks**

Si el valor es null, o no se establece una LICENSE válida, se usará la cadena Aspose.Cells vVERSION.

**Returns:**
java.lang.String
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica si se almacena en caché los datos más recientes del gráfico.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Obtiene los comportamientos de renderizado específicos de Excel a aplicar.

Ver [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

El valor predeterminado es [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el formato de archivo guardado.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Establezca estas opciones, cuando se necesite seguridad en el resultado xls2pdf.

**Example**

El siguiente código establece la resolución de altura de impresión para el PDF de salida.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtiene las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

El siguiente código solo renderiza la hoja activa a PDF.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Obtiene el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda.

Ver [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
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
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Obtiene la marca de agua para la salida.

**Example**

El siguiente código establece la marca de agua en el PDF de salida.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Obtiene el modo de vista inicial cuando se abre el documento PDF generado. El valor predeterminado es [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Ver [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Obtiene el porcentaje de zoom usado cuando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) es [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Esta propiedad se ignora a menos que [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) sea [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella.

**Remarks**

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Workbook y PdfSaveOption/system para la fuente de la celda.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


Establece el objeto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

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


Indica si se deben calcular las fórmulas antes de guardar el archivo pdf.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando ingresa un valor más largo que 32K, se truncará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto.

**Remarks**

El valor predeterminado es verdadero. Desactivar esta propiedad puede ofrecer mejor rendimiento. Pero cuando la fuente predeterminada o especificada del texto/carácter no puede usarse para renderizarlo, pueden aparecer caracteres ilegibles (como bloques) en el PDF generado. En tal situación el usuario debe mantener esta propiedad como verdadera para que se busque y use una fuente alternativa para renderizar el texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar primero estos caracteres.

**Remarks**

El valor predeterminado es verdadero.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Establece el nivel de cumplimiento de los estándares PDF para los documentos de salida.

Ver [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

El valor predeterminado es Pdf17.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Establece la hora de generación del documento pdf.

**Remarks**

Si no se establece, será la hora de generar el PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


Establece un valor que determina la forma en que [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) se exporta al archivo PDF. El valor predeterminado es None.

Ver [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Establece configuraciones personalizadas durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Establece el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, establezca la DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Indica si la barra de título de la ventana debe mostrar el título del documento.

**Remarks**

Si es false, la barra de título debe mostrar en su lugar el nombre del archivo PDF. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Indica si se debe incrustar el adjunto para objetos Ole en Excel.

**Remarks**

El valor predeterminado es false. El valor debe ser false cuando se establece la conformidad PDF/A o el cifrado PDF está habilitado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True para incrustar fuentes TrueType. Afecta solo a los caracteres ASCII 32-127. Las fuentes para códigos de caracteres mayores a 127 siempre se incrustan. Las fuentes siempre se incrustan para el estándar PDF/A-1a, PDF/A-1b. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Configuración para renderizar un metafichero Emf.

Ver [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando se establece [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), los registros EMF+ se analizarán al renderizar la página; de lo contrario solo se analizarán los registros EMF. El valor predeterminado es [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Indica si se debe exportar la estructura del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


Establece la codificación de fuentes incrustadas en pdf.

Ver [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

El valor predeterminado es [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella.

**Remarks**

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Workbook y PdfSaveOption/system para la fuente de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Establece el color de la línea de cuadrícula.

**Remarks**

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Establece el tipo de línea de cuadrícula.

Ver [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

El valor predeterminado es tipo punteado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indica si necesita ocultar el error durante la renderización. El error puede ser en forma, imagen, renderizado de gráfico, etc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Establece los PPI (píxeles por pulgada) deseados para el remuestreo de imágenes y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada, y las imágenes que superen los PPI especificados (píxeles por pulgada) serán remuestreadas.

**Example**

El siguiente código establece los PPI deseados en 96 y la calidad JPEG en 80 para las imágenes del PDF de salida.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredPPI | int | Píxeles por pulgada deseados. 220 alta calidad. 150 calidad de pantalla. 96 calidad de correo electrónico. |
| jpegQuality | int | Calidad JPEG 0 - 100%. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Representa el tipo de imagen al convertir el gráfico y la forma.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad del renderizado. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán aplicándose.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


Establece el tipo de optimización pdf.

Ver [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

El valor predeterminado es [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

**Remarks**

El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Establece el número de páginas a guardar.

**Remarks**

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Establece el índice basado en cero de la primera página a guardar.

**Remarks**

El valor predeterminado es 0.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Controla/Indica el progreso del proceso de guardado de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Indica el algoritmo de compresión

Ver [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Indica qué páginas no se imprimirán.

Ver [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Si el contenido de la hoja es escaso, algunas páginas pueden quedar totalmente en blanco en el archivo PDF de salida. Si no deseas esas páginas en blanco, puedes usar esta opción para omitirlas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Establece el productor del documento pdf generado.

**Remarks**

Si el valor es null, o no se establece una LICENSE válida, se usará la cadena Aspose.Cells vVERSION.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica si se almacena en caché los datos más recientes del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Establece los comportamientos de renderizado específicos de Excel a aplicar.

Ver [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

El valor predeterminado es [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


Establezca estas opciones, cuando se necesite seguridad en el resultado xls2pdf.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Establece las hojas a renderizar. El predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Establece el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda.

Ver [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Establece la marca de agua en la salida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Establece el modo de vista inicial cuando se abre el documento PDF generado. El valor predeterminado es [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Ver [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Establece el porcentaje de zoom usado cuando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) es [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Esta propiedad se ignora a menos que [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) sea [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

