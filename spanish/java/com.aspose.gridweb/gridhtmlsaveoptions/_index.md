---
title: "GridHtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para guardar el archivo html."
type: docs
url: /es/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Representa las opciones para guardar el archivo html.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Crea opciones para guardar un archivo html. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Crea opciones para guardar un archivo htm. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | El directorio donde se guardarán los archivos adjuntos. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta de archivos en caché se usa para almacenar datos grandes. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getDefaultFontName()](#getDefaultFontName--) | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null. |
| [getEncoding()](#getEncoding--) | Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indica si se exporta todo el libro de trabajo a un archivo html. |
| [getExportArea()](#getExportArea--) | Obtiene el CellArea de exportación de la hoja de cálculo activa actual. |
| [getExportGridLines()](#getExportGridLines--) | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [getExportHeadings()](#getExportHeadings--) | Indica si se exportan los encabezados al guardar el archivo en html. El valor predeterminado es false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indica si solo se exporta el área de impresión al archivo html. |
| [getExportSingleTab()](#getExportSingleTab--) | Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getPageTitle()](#getPageTitle--) | El título de la página HTML. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Analizar etiqueta html en la celda, como |

, como valor de celda, o como etiqueta html, el valor predeterminado es true |
| [getPresentationPreference()](#getPresentationPreference--) | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se está refrescando los datos de caché del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [isFullPathLink()](#isFullPathLink--) | Indicando si se utiliza enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | El directorio donde se guardarán los archivos adjuntos. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta de archivos en caché se usa para almacenar datos grandes. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indica si se exporta todo el libro de trabajo a un archivo html. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Establece el CellArea de exportación de la Worksheet activa actual. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indica si se exportan los encabezados al guardar el archivo en html. El valor predeterminado es false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indica si solo se exporta el área de impresión al archivo html. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indica si se exporta la única pestaña cuando el archivo solo tiene una hoja de cálculo. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indicando si se utiliza enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | El título de la página HTML. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Analizar etiqueta html en la celda, como |

, como valor de celda, o como etiqueta html, el valor predeterminado es true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se está refrescando los datos de caché del gráfico. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Crea opciones para guardar un archivo html.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Crea opciones para guardar un archivo htm.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). El formato de archivo de guardado. |

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


La carpeta de archivos en caché se usa para almacenar datos grandes.

**Returns:**
java.lang.String
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indica si se exporta todo el libro de trabajo a un archivo html.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Obtiene el CellArea de exportación de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja de cálculo activa actual se omitirá. Solo el área especificada se exportará al guardar el archivo en html.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
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


Indica si se exportan los encabezados al guardar el archivo en html. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.

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
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false.

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


Analizar etiqueta html en la celda, como

, como valor de celda, o como etiqueta html, el valor predeterminado es true

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


Indica si se está refrescando los datos de caché del gráfico.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el formato de archivo guardado.

Ver [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica si se ordenan los nombres definidos antes de guardar el archivo.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La carpeta de archivos en caché se usa para almacenar datos grandes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es nula, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original; el valor predeterminado es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Si no se establece, se usa Encoding.UTF8 como tipo de codificación predeterminado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indica si se exporta todo el libro de trabajo a un archivo html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Establece el CellArea de exportación de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja de cálculo activa actual se omitirá. Solo el área especificada se exportará al guardar el archivo en html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false.

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


Indica si se exportan los encabezados al guardar el archivo en html. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado.

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

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false.

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

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indica si se utiliza un enlace de ruta completa en sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false.

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


Analizar etiqueta html en la celda, como

, como valor de celda, o como etiqueta html, el valor predeterminado es true

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


Indica si se está refrescando los datos de caché del gráfico.

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

