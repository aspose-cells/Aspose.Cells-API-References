---
title: "XmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de guardar el libro de trabajo como un archivo xml."
type: docs
url: /es/java/com.aspose.cells/xmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class XmlSaveOptions extends SaveOptions
```

Representa las opciones de guardar el libro de trabajo como un archivo xml.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XmlSaveOptions()](#XmlSaveOptions--) | Crea opciones para guardar un archivo XML. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getDataAsAttribute()](#getDataAsAttribute--) | Indica si se exportan datos como atributos del elemento. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExportArea()](#getExportArea--) | Obtiene el rango de exportación. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSheetIndexes()](#getSheetIndexes--) | Representa los índices de las hojas exportadas. |
| [getSheetNameAsElementName()](#getSheetNameAsElementName--) | Indica si se exporta el nombre de la hoja como el nombre del elemento. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [getXmlMapName()](#getXmlMapName--) | Indica si se exporta el mapa xml en el archivo. |
| [hasHeaderRow()](#hasHeaderRow--) | Indica si el rango contiene una fila de encabezado. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setDataAsAttribute(boolean value)](#setDataAsAttribute-boolean-) | Indica si se exportan datos como atributos del elemento. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Establece el rango de exportación. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indica si el rango contiene una fila de encabezado. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Representa los índices de las hojas exportadas. |
| [setSheetNameAsElementName(boolean value)](#setSheetNameAsElementName-boolean-) | Indica si se exporta el nombre de la hoja como el nombre del elemento. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [setXmlMapName(String value)](#setXmlMapName-java.lang.String-) | Indica si se exporta el mapa xml en el archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlSaveOptions() {#XmlSaveOptions--}
```
public XmlSaveOptions()
```


Crea opciones para guardar un archivo XML.

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
### getDataAsAttribute() {#getDataAsAttribute--}
```
public boolean getDataAsAttribute()
```


Indica si se exportan datos como atributos del elemento.

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
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Obtiene el rango de exportación.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Representa los índices de las hojas exportadas.

**Returns:**
int[]
### getSheetNameAsElementName() {#getSheetNameAsElementName--}
```
public boolean getSheetNameAsElementName()
```


Indica si se exporta el nombre de la hoja como el nombre del elemento.

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
### getXmlMapName() {#getXmlMapName--}
```
public String getXmlMapName()
```


Indica si se exporta el mapa xml en el archivo.

**Returns:**
java.lang.String
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Indica si el rango contiene una fila de encabezado.

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

### setDataAsAttribute(boolean value) {#setDataAsAttribute-boolean-}
```
public void setDataAsAttribute(boolean value)
```


Indica si se exportan datos como atributos del elemento.

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

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Establece el rango de exportación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indica si el rango contiene una fila de encabezado.

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica si se almacena en caché los datos más recientes del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Representa los índices de las hojas exportadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

### setSheetNameAsElementName(boolean value) {#setSheetNameAsElementName-boolean-}
```
public void setSheetNameAsElementName(boolean value)
```


Indica si se exporta el nombre de la hoja como el nombre del elemento.

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

### setXmlMapName(String value) {#setXmlMapName-java.lang.String-}
```
public void setXmlMapName(String value)
```


Indica si se exporta el mapa xml en el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

