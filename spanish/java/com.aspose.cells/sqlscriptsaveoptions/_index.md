---
title: "SqlScriptSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de guardado de sql."
type: docs
url: /es/java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

Representa las opciones de guardado de sql.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | Crea opciones para guardar el archivo sql. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | Inserta una línea en blanco entre cada dato. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | Verifica todos los datos para encontrar el tipo de datos de las columnas. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | Comprueba si el nombre de la tabla existe antes de crearla. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getColumnTypeMap()](#getColumnTypeMap--) | Obtiene el mapa de tipos de columna para diferentes bases de datos. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getCreateTable()](#getCreateTable--) | Indica si se exporta sql para crear la tabla. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExportArea()](#getExportArea--) | Obtiene el rango de exportación. |
| [getExportAsString()](#getExportAsString--) | Indica si se exportan todos los datos como valores de cadena. |
| [getIdName()](#getIdName--) | Obtiene el nombre de la columna id. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getOperatorType()](#getOperatorType--) | Obtiene el tipo de operador del sql. |
| [getPrimaryKey()](#getPrimaryKey--) | Representa cuál columna es la clave primaria de la tabla de datos. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSeparator()](#getSeparator--) | Obtiene el separador de caracteres del script sql. |
| [getSheetIndexes()](#getSheetIndexes--) | Representa los índices de las hojas exportadas. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getStartId()](#getStartId--) | Obtiene el id inicial. |
| [getTableName()](#getTableName--) | Obtiene el nombre de la tabla. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hasHeaderRow()](#hasHeaderRow--) | Indica si el rango contiene una fila de encabezado. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | Inserta una línea en blanco entre cada dato. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | Verifica todos los datos para encontrar el tipo de datos de las columnas. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | Comprueba si el nombre de la tabla existe antes de crearla. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | Establece el mapa de tipos de columna para diferentes bases de datos. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | Indica si se exporta sql para crear la tabla. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Establece el rango de exportación. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Indica si se exportan todos los datos como valores de cadena. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indica si el rango contiene una fila de encabezado. |
| [setIdName(String value)](#setIdName-java.lang.String-) | Establece el nombre de la columna id. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setOperatorType(int value)](#setOperatorType-int-) | Establece el tipo de operador del sql. |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | Representa cuál columna es la clave primaria de la tabla de datos. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSeparator(char value)](#setSeparator-char-) | Establece el separador de caracteres del script sql. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Representa los índices de las hojas exportadas. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setStartId(int value)](#setStartId-int-) | Establece el id inicial. |
| [setTableName(String value)](#setTableName-java.lang.String-) | Establece el nombre de la tabla. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


Crea opciones para guardar el archivo sql.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


Inserta una línea en blanco entre cada dato.

**Remarks**

Si [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) es '\\n', es mejor establecer esta propiedad como true para aumentar la legibilidad.

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
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


Verifica todos los datos para encontrar el tipo de datos de las columnas.

**Remarks**

El valor predeterminado es false, solo verificamos la primera fila por rendimiento. Si esta propiedad es true y las columnas contienen tipos de valor mixtos, el tipo de las columnas será texto.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando ingresa un valor más largo que 32K, se truncará.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


Comprueba si el nombre de la tabla existe antes de crearla.

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
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


Obtiene el mapa de tipos de columna para diferentes bases de datos.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


Indica si se exporta sql para crear la tabla.

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
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Indica si se exportan todos los datos como valores de cadena.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


Obtiene el nombre de la columna id.

**Remarks**

Si se establece esta propiedad, se insertará una columna con un valor entero de incremento automático.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


Obtiene el tipo de operador del sql.

Ver [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


Representa cuál columna es la clave primaria de la tabla de datos.

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Obtiene el separador de caracteres del script sql.

**Remarks**

Solo puede ser ' ' o '\\n'. Si el

**Returns:**
char
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Representa los índices de las hojas exportadas.

**Returns:**
int[]
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
### getStartId() {#getStartId--}
```
public int getStartId()
```


Obtiene el id inicial.

**Remarks**

Solo funciona cuando [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) está configurado.

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


Obtiene el nombre de la tabla.

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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


Inserta una línea en blanco entre cada dato.

**Remarks**

Si [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) es '\\n', es mejor establecer esta propiedad como true para aumentar la legibilidad.

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

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


Verifica todos los datos para encontrar el tipo de datos de las columnas.

**Remarks**

El valor predeterminado es false, solo verificamos la primera fila por rendimiento. Si esta propiedad es true y las columnas contienen tipos de valor mixtos, el tipo de las columnas será texto.

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

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


Comprueba si el nombre de la tabla existe antes de crearla.

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

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


Establece el mapa de tipos de columna para diferentes bases de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

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

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


Indica si se exporta sql para crear la tabla.

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

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Indica si se exportan todos los datos como valores de cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indica si el rango contiene una fila de encabezado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


Establece el nombre de la columna id.

**Remarks**

Si se establece esta propiedad, se insertará una columna con un valor entero de incremento automático.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


Establece el tipo de operador del sql.

Ver [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


Representa cuál columna es la clave primaria de la tabla de datos.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Establece el separador de caracteres del script sql.

**Remarks**

Solo puede ser ' ' o '\\n'. Si el

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Representa los índices de las hojas exportadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

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

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


Establece el id inicial.

**Remarks**

Solo funciona cuando [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) está configurado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


Establece el nombre de la tabla.

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

