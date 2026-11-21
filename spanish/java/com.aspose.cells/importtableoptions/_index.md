---
title: "ImportTableOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de importación de datos en celdas."
type: docs
url: /es/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Representa las opciones de importación de datos en celdas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Crea las opciones de importación predeterminadas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Indica si se verifica la fusión de celdas. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Obtiene las columnas (basadas en 0) para importar del origen de datos. null significa que se deben importar todas las columnas. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Indica si se aplica el estilo de la vista de cuadrícula a las celdas. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtiene un valor que indica si el valor de cadena debe convertirse a numérico o a fecha. |
| [getDateFormat()](#getDateFormat--) | Obtiene la cadena de formato de fecha para celdas con valores de fecha y hora importados. |
| [getDefaultValues()](#getDefaultValues--) | El valor predeterminado para el valor en la tabla es null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Indica si se exporta el título como nombre de campo |
| [getInsertRows()](#getInsertRows--) | Indica si se deben agregar nuevas filas para importar registros de datos. |
| [getNumberFormats()](#getNumberFormats--) | Obtiene los formatos numéricos |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Indica si se desplaza la primera fila hacia abajo al insertar filas. |
| [getStyles()](#getStyles--) | Obtiene los estilos para cada columna de la tabla. |
| [getTotalColumns()](#getTotalColumns--) | Obtiene el recuento total de columnas para importar del origen de datos. -1 significa todas las filas del origen de datos dado. |
| [getTotalRows()](#getTotalRows--) | Obtiene el recuento total de filas para importar del origen de datos. -1 significa todas las filas del origen de datos dado. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Indica si el nombre de campo debe ser importado. |
| [isFormulas()](#isFormulas--) | Indica si los datos son fórmulas. |
| [isHtmlString()](#isHtmlString--) | Indica si el valor contiene etiquetas html. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Indica si se verifica la fusión de celdas. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Establece las columnas (basadas en 0) que se importarán del origen de datos. null significa que se deben importar todas las columnas. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Indica si se aplica el estilo de la vista de cuadrícula a las celdas. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Establece un valor que indica si el valor de cadena debe convertirse a valor numérico o de fecha. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Establece la cadena de formato de fecha para celdas con valores de fecha y hora importados. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | El valor predeterminado para el valor en la tabla es null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Indica si se exporta el título como nombre de campo |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Indica si el nombre de campo debe ser importado. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Indica si los datos son fórmulas. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Indica si el valor contiene etiquetas html. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Indica si se deben agregar nuevas filas para importar registros de datos. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Establece los formatos numéricos |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Indica si se desplaza la primera fila hacia abajo al insertar filas. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Establece los estilos para cada columna de la tabla. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Establece el recuento total de columnas a importar del origen de datos. -1 significa todas las filas del origen de datos dado. |
| [setTotalRows(int value)](#setTotalRows-int-) | Establece el recuento total de filas a importar del origen de datos. -1 significa todas las filas del origen de datos dado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Crea las opciones de importación predeterminadas.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Indica si se verifica la fusión de celdas.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Obtiene las columnas (basadas en 0) para importar del origen de datos. null significa que se deben importar todas las columnas.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Indica si se aplica el estilo de la vista de cuadrícula a las celdas.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtiene un valor que indica si el valor de cadena debe convertirse a numérico o a fecha.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Obtiene la cadena de formato de fecha para celdas con valores de fecha y hora importados.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


El valor predeterminado para el valor en la tabla es null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Indica si se exporta el título como nombre de campo

**Remarks**

Solo funciona con DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Indica si se deben agregar nuevas filas para importar registros de datos.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Obtiene los formatos numéricos

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Indica si se desplaza la primera fila hacia abajo al insertar filas.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Obtiene los estilos para cada columna de la tabla.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Obtiene el recuento total de columnas para importar del origen de datos. -1 significa todas las filas del origen de datos dado.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Obtiene el recuento total de filas para importar del origen de datos. -1 significa todas las filas del origen de datos dado.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Indica si el nombre de campo debe ser importado.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Indica si los datos son fórmulas.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Indica si el valor contiene etiquetas html.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Indica si se verifica la fusión de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Establece las columnas (basadas en 0) que se importarán del origen de datos. null significa que se deben importar todas las columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Indica si se aplica el estilo de la vista de cuadrícula a las celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Establece un valor que indica si el valor de cadena debe convertirse a valor numérico o de fecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Establece la cadena de formato de fecha para celdas con valores de fecha y hora importados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


El valor predeterminado para el valor en la tabla es null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Indica si se exporta el título como nombre de campo

**Remarks**

Solo funciona con DataTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Indica si el nombre de campo debe ser importado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Indica si los datos son fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Indica si el valor contiene etiquetas html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Indica si se deben agregar nuevas filas para importar registros de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Establece los formatos numéricos

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Indica si se desplaza la primera fila hacia abajo al insertar filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Establece los estilos para cada columna de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Establece el recuento total de columnas a importar del origen de datos. -1 significa todas las filas del origen de datos dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Establece el recuento total de filas a importar del origen de datos. -1 significa todas las filas del origen de datos dado.

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

