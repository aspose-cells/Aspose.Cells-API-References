---
title: "OoxmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de guardado del archivo Office Open XML."
type: docs
url: /es/java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Representa las opciones de guardado del archivo Office Open XML.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Crea las opciones para guardar un archivo Office Open XML. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Crea las opciones para guardar un archivo Office Open XML. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAsFlatOpc()](#getAsFlatOpc--) | Indica si se guarda como un archivo OPC plano que puede ser generado por Open XML SDK. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCompressionType()](#getCompressionType--) | Obtiene el tipo de compresión para el archivo ooxml. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Indica si se incrustan archivos Ooxml de OleObject como objeto ole. |
| [getEnableZip64()](#getEnableZip64--) | Utiliza extensiones ZIP64 al escribir archivos zip, según sea necesario. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExportCellName()](#getExportCellName--) | Indica si exportar el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getUpdateZoom()](#getUpdateZoom--) | Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indica si se debe hacer el xls más compatible con WPS. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Indica si se guarda como un archivo OPC plano que puede ser generado por Open XML SDK. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCompressionType(int value)](#setCompressionType-int-) | Establece el tipo de compresión para el archivo ooxml. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Indica si se incrustan archivos Ooxml de OleObject como objeto ole. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Utiliza extensiones ZIP64 al escribir archivos zip, según sea necesario. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Indica si exportar el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indica si se debe hacer el xls más compatible con WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Crea las opciones para guardar un archivo Office Open XML.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Crea las opciones para guardar un archivo Office Open XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de archivo. Debe ser uno de los siguientes tipos: [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX), [SaveFormat.XLTX](../../com.aspose.cells/saveformat\#XLTX), [SaveFormat.XLAM](../../com.aspose.cells/saveformat\#XLAM), [SaveFormat.XLSM](../../com.aspose.cells/saveformat\#XLSM) o [SaveFormat.XLTM](../../com.aspose.cells/saveformat\#XLTM), de lo contrario el formato guardado se establecerá como [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX) automáticamente. |

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
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Indica si se guarda como un archivo OPC plano que puede ser generado por Open XML SDK.

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
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Obtiene el tipo de compresión para el archivo ooxml.

Vea [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

El valor predeterminado es OoxmlCompressionType.Level2.

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
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Indica si se incrustan archivos Ooxml de OleObject como objeto ole.

**Remarks**

Solo para OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Utiliza extensiones ZIP64 al escribir archivos zip, según sea necesario.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true.

**Remarks**

Solo para archivos .xls, .xlsx, .xlsb y .xlsm.

**Returns:**
boolean
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Indica si exportar el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si el archivo de salida puede ser accedido por SQL Server DTS, este valor debe ser verdadero. Establecer el valor en falso aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear archivos grandes. El valor predeterminado es verdadero.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


El proveedor de datos para guardar el libro de trabajo en modo ligero.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica si se almacena en caché los datos más recientes del gráfico.

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
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica si se actualiza la configuración de SmartArt. El valor predeterminado es false.

**Remarks**

Solo tiene efecto después de llamar al método Shape.GetResultOfSmartArt() y cuando las formas en caché existen en el archivo de plantilla.

**Returns:**
boolean
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo.

**Remarks**

El valor predeterminado es falso por rendimiento.

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
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indica si se debe hacer el xls más compatible con WPS.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookSetting.WpsCompatibility. Este método será eliminado 12 meses después, a partir de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Indica si se guarda como un archivo OPC plano que puede ser generado por Open XML SDK.

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

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Deja el libro de trabajo vacío después de guardar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Establece el tipo de compresión para el archivo ooxml.

Vea [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

El valor predeterminado es OoxmlCompressionType.Level2.

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

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Indica si se incrustan archivos Ooxml de OleObject como objeto ole.

**Remarks**

Solo para OleObject.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Utiliza extensiones ZIP64 al escribir archivos zip, según sea necesario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Indica si exportar el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si el archivo de salida puede ser accedido por SQL Server DTS, este valor debe ser verdadero. Establecer el valor en falso aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear archivos grandes. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


El proveedor de datos para guardar el libro de trabajo en modo ligero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica si se almacena en caché los datos más recientes del gráfico.

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

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo.

**Remarks**

El valor predeterminado es falso por rendimiento.

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

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indica si se debe hacer el xls más compatible con WPS.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookSetting.WpsCompatibility. Este método será eliminado 12 meses después, a partir de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

