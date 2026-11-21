---
title: "TxtSaveOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de guardado para formato csv/tab delimitado/u otro formato de texto."
type: docs
url: /es/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

Representa las opciones de guardado para formato csv/tab delimitado/u otro formato de texto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Crea opciones de guardado de archivo de texto. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Crea opciones de guardado de archivo de texto. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Indica si siempre se agrega '\\"' para cada campo. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [getCreateDirectory()](#getCreateDirectory--) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [getEncoding()](#getEncoding--) | Obtiene la codificación predeterminada. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [getExportAllSheets()](#getExportAllSheets--) | Indica si se exportan todas las hojas al archivo de texto. |
| [getExportArea()](#getExportArea--) | El rango de celdas a exportar. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) es verdadero para ella. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtiene la estrategia de formato al exportar el valor de la celda como cadena. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Indica si se deben generar separadores para una fila en blanco. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [getMergeAreas()](#getMergeAreas--) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [getQuoteType()](#getQuoteType--) | Obtiene cómo citar los valores en el archivo de texto exportado. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el formato de archivo guardado. |
| [getSeparator()](#getSeparator--) | Obtiene el carácter delimitador del archivo de texto. |
| [getSeparatorString()](#getSeparatorString--) | Obtiene un valor de cadena como separador. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [getSortNames()](#getSortNames--) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace MS Excel. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Indica si las celdas en blanco finales en una fila deben recortarse. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica si se actualiza la configuración de SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Indica si siempre se agrega '\\"' para cada campo. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setClearData(boolean value)](#setClearData-boolean-) | Deja el libro de trabajo vacío después de guardar el archivo. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Establece la codificación predeterminada. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Indica si se exportan todas las hojas al archivo de texto. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | El rango de celdas a exportar. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) es verdadero para ella. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Indica si se deben generar separadores para una fila en blanco. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo. |
| [setQuoteType(int value)](#setQuoteType-int-) | Establece cómo citar los valores en el archivo de texto exportado. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica si se almacena en caché los datos más recientes del gráfico. |
| [setSeparator(char value)](#setSeparator-char-) | Establece el carácter delimitador del archivo de texto. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Establece un valor de cadena como separador. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica si se ordenan los nombres definidos externos antes de guardar el archivo. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica si se ordenan los nombres definidos antes de guardar el archivo. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace MS Excel. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Indica si las celdas en blanco finales en una fila deben recortarse. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica si se actualiza la configuración de SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica si se validan las celdas combinadas antes de guardar el archivo. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Crea opciones de guardado de archivo de texto.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


Crea opciones de guardado de archivo de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El formato de archivo. Debe ser [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV) o [SaveFormat.TSV](../../com.aspose.cells/saveformat\\#TSV), de lo contrario el formato guardado se establecerá automáticamente como [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV). |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Indica si siempre se agrega '\\"' para cada campo. Si es verdadero, todos los valores se citarán; si es falso, los valores solo se citarán cuando sea necesario (por ejemplo, cuando los valores contengan caracteres especiales como '\\"', '\\\\n' o el carácter separador). El valor predeterminado es falso.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad QuoteType. Esta propiedad será eliminada 12 meses después a partir de agosto de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtiene la codificación predeterminada.

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
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Indica si se exportan todas las hojas al archivo de texto. Si es falso, solo se exporta la hoja activa, como en MS Excel.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


El rango de celdas a exportar.

**Remarks**

Si se ha especificado el área exportada, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) no tendrá efecto.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) es verdadero para ella. El valor predeterminado es false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtiene la estrategia de formato al exportar el valor de la celda como cadena.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es false, por lo que por defecto el contenido de la fila en blanco será vacío.

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
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Obtiene cómo citar los valores en el archivo de texto exportado.

Ver [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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


Obtiene el carácter delimitador del archivo de texto.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Obtiene un valor de cadena como separador.

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


Indica si se deben recortar las filas y columnas en blanco iniciales como lo hace MS Excel. El valor predeterminado es true.

**Remarks**

Igual que la regla en MS Excel, una fila/columna no se considerará en blanco si tiene un estilo personalizado, incluso si no contiene datos de celda. Al guardar en modo LightCells, esta opción no tiene efecto. El usuario debe controlar el rango de salida mediante la implementación de [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) o especificando [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Indica si se deben recortar las celdas en blanco finales en una fila. El valor predeterminado es false.

**Remarks**

Al guardar en modo LightCells y no haberse especificado [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--), esta opción no tiene efecto y una fila se extenderá hasta la última celda proporcionada por la implementación [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Indica si siempre se agrega '\\"' para cada campo. Si es verdadero, todos los valores se citarán; si es falso, los valores solo se citarán cuando sea necesario (por ejemplo, cuando los valores contengan caracteres especiales como '\\"', '\\\\n' o el carácter separador). El valor predeterminado es falso.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad QuoteType. Esta propiedad será eliminada 12 meses después a partir de agosto de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Establece la codificación predeterminada.

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Indica si se exportan todas las hojas al archivo de texto. Si es falso, solo se exporta la hoja activa, como en MS Excel.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


El rango de celdas a exportar.

**Remarks**

Si se ha especificado el área exportada, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) no tendrá efecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) es verdadero para ella. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Establece la estrategia de formato al exportar el valor de la celda como cadena.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es false, por lo que por defecto el contenido de la fila en blanco será vacío.

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Establece cómo citar los valores en el archivo de texto exportado.

Ver [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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


Establece el carácter delimitador del archivo de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Establece un valor de cadena como separador.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


Indica si se deben recortar las filas y columnas en blanco iniciales como lo hace MS Excel. El valor predeterminado es true.

**Remarks**

Igual que la regla en MS Excel, una fila/columna no se considerará en blanco si tiene un estilo personalizado, incluso si no contiene datos de celda. Al guardar en modo LightCells, esta opción no tiene efecto. El usuario debe controlar el rango de salida mediante la implementación de [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) o especificando [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Indica si se deben recortar las celdas en blanco finales en una fila. El valor predeterminado es false.

**Remarks**

Al guardar en modo LightCells y no haberse especificado [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--), esta opción no tiene efecto y una fila se extenderá hasta la última celda proporcionada por la implementación [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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

