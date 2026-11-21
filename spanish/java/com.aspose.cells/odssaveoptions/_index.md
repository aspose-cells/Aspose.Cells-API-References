---
title: "OdsSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de guardado del archivo ods."
type: docs
url: /es/java/com.aspose.cells/odssaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OdsSaveOptions extends SaveOptions
```

Representa las opciones de guardado del archivo ods.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OdsSaveOptions()](#OdsSaveOptions--) | Crea las opciones de guardado del archivo ods. |
| [OdsSaveOptions(int saveFormat)](#OdsSaveOptions-int-) | Crea las opciones de guardado del archivo ods. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getGeneratorType()](#getGeneratorType--) | Obtiene el generador del archivo ods. |
| [getIgnorePivotTables()](#getIgnorePivotTables--) | Indica si se guardan las tablas dinámicas. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getOdfStrictVersion()](#getOdfStrictVersion--) | Obtiene la versión ODF. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hashCode()](#hashCode--) |  |
| [isStrictSchema11()](#isStrictSchema11--) | Indica si el archivo ods debe guardarse como versión 1.1 del formato ODF. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setGeneratorType(int value)](#setGeneratorType-int-) | Establece el generador del archivo ods. |
| [setIgnorePivotTables(boolean value)](#setIgnorePivotTables-boolean-) | Indica si se guardan las tablas dinámicas. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setOdfStrictVersion(int value)](#setOdfStrictVersion-int-) | Establece la versión ODF. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setStrictSchema11(boolean value)](#setStrictSchema11-boolean-) | Indica si el archivo ods debe guardarse como versión 1.1 del formato ODF. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OdsSaveOptions() {#OdsSaveOptions--}
```
public OdsSaveOptions()
```


Crea las opciones de guardado del archivo ods.

### OdsSaveOptions(int saveFormat) {#OdsSaveOptions-int-}
```
public OdsSaveOptions(int saveFormat)
```


Crea las opciones de guardado del archivo ods.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de archivo. Debe ser [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS), [SaveFormat.OTS](../../com.aspose.cells/saveformat\#OTS), [SaveFormat.FODS](../../com.aspose.cells/saveformat\#FODS) o [SaveFormat.SXC](../../com.aspose.cells/saveformat\#SXC), de lo contrario el formato guardado se establecerá automáticamente como [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS). |

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

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
### getGeneratorType() {#getGeneratorType--}
```
public int getGeneratorType()
```


Obtiene el generador del archivo ods.

Ver [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype).

**Returns:**
int
### getIgnorePivotTables() {#getIgnorePivotTables--}
```
public boolean getIgnorePivotTables()
```


Indica si se guardan las tablas dinámicas.

**Remarks**

La función de tabla dinámica de OpenOffice tiene menos configuraciones en comparación con Excel, por lo que sus resultados de tabla dinámica presentan muchas diferencias. A veces es mejor ignorar estas tablas dinámicas al guardar un archivo .ods.

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
### getOdfStrictVersion() {#getOdfStrictVersion--}
```
public int getOdfStrictVersion()
```


Obtiene la versión ODF.

Ver [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype).

**Returns:**
int
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
### isStrictSchema11() {#isStrictSchema11--}
```
public boolean isStrictSchema11()
```


Indica si el archivo ods debe guardarse como ODF versión 1.1. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad OdsSaveOptions.OdfStrictVersion. Este método será eliminado 12 meses después de febrero de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

### setGeneratorType(int value) {#setGeneratorType-int-}
```
public void setGeneratorType(int value)
```


Establece el generador del archivo ods.

Ver [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIgnorePivotTables(boolean value) {#setIgnorePivotTables-boolean-}
```
public void setIgnorePivotTables(boolean value)
```


Indica si se guardan las tablas dinámicas.

**Remarks**

La función de tabla dinámica de OpenOffice tiene menos configuraciones en comparación con Excel, por lo que sus resultados de tabla dinámica presentan muchas diferencias. A veces es mejor ignorar estas tablas dinámicas al guardar un archivo .ods.

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

### setOdfStrictVersion(int value) {#setOdfStrictVersion-int-}
```
public void setOdfStrictVersion(int value)
```


Establece la versión ODF.

Ver [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype).

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

### setStrictSchema11(boolean value) {#setStrictSchema11-boolean-}
```
public void setStrictSchema11(boolean value)
```


Indica si el archivo ods debe guardarse como ODF versión 1.1. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad OdsSaveOptions.OdfStrictVersion. Este método será eliminado 12 meses después de febrero de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

