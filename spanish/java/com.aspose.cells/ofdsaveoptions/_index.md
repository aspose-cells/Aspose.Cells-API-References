---
title: "OfdSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para guardar un archivo OFDOpen Fixed-layout Document."
type: docs
url: /es/java/com.aspose.cells/ofdsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class OfdSaveOptions extends PaginatedSaveOptions
```

Representa las opciones para guardar un archivo OFD (Open Fixed-layout Document).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OfdSaveOptions()](#OfdSaveOptions--) | Crea las opciones para guardar el archivo OFD. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtiene configuraciones personalizadas durante el renderizado. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtiene el idioma de edición predeterminado. |
| [getDefaultFont()](#getDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Configuración para renderizar un metafichero Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getGridlineColor()](#getGridlineColor--) | Obtiene el color de la línea de cuadrícula. |
| [getGridlineType()](#getGridlineType--) | Obtiene el tipo de línea de cuadrícula. |
| [getIgnoreError()](#getIgnoreError--) | Indica si necesita ocultar el error durante el renderizado. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [getPageCount()](#getPageCount--) | Obtiene el número de páginas a guardar. |
| [getPageIndex()](#getPageIndex--) | Obtiene el índice basado en cero de la primera página a guardar. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controla/Indica el progreso del proceso de guardado de página. |
| [getPrintingPageType()](#getPrintingPageType--) | Indica qué páginas no se imprimirán. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Obtiene los comportamientos de renderizado específicos de Excel a aplicar. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSheetSet()](#getSheetSet--) | Obtiene las hojas a renderizar. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getTextCrossType()](#getTextCrossType--) | Obtiene el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Establece configuraciones personalizadas durante la renderización. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Establece el idioma de edición predeterminado. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Configuración para renderizar un metafichero Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Establece el color de la línea de cuadrícula. |
| [setGridlineType(int value)](#setGridlineType-int-) | Establece el tipo de línea de cuadrícula. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica si necesita ocultar el error durante el renderizado. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [setPageCount(int value)](#setPageCount-int-) | Establece el número de páginas a guardar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Establece el índice basado en cero de la primera página a guardar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controla/Indica el progreso del proceso de guardado de página. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indica qué páginas no se imprimirán. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Establece los comportamientos de renderizado específicos de Excel a aplicar. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Establece las hojas a renderizar. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Establece el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OfdSaveOptions() {#OfdSaveOptions--}
```
public OfdSaveOptions()
```


Crea las opciones para guardar el archivo OFD.

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La carpeta para archivos temporales que pueden usarse como caché de datos.

**Remarks**

Si no se ha especificado la carpeta, el valor predeterminado es [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si su valor predeterminado es nulo o está vacío, o se ha especificado como nulo o vacío, entonces no se utilizará ningún archivo de caché al guardar el libro de trabajo.

**Returns:**
java.lang.String
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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
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
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
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

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

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

