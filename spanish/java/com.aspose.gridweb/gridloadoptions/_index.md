---
title: "GridLoadOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de carga del archivo."
type: docs
url: /es/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

Representa las opciones de carga del archivo. [Obsolete("Esta clase quedará obsoleta después del uso independiente de dll de la API pública de cells, en su lugar puede usar Aspose.Cells.LodOptions ")]
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | Crea una opción de carga del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [getCheckDataValid()](#getCheckDataValid--) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [getOnlyAuto()](#getOnlyAuto--) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica si se analiza la fórmula al leer el archivo. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [getPassword()](#getPassword--) | Obtiene la contraseña del libro de trabajo. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica si se analiza la fórmula al leer el archivo. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Establece la contraseña del workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


Crea una opción de carga del archivo.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indica si se filtra automáticamente los datos al cargar los archivos.

**Remarks**

A veces, aunque el autofiltro está configurado, las filas correspondientes no se ocultan en el archivo. Ahora solo funciona para archivos SpreadSheetML.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Comprueba si los datos son válidos en el archivo de plantilla.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si la propiedad es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que no es válido para el formato de archivo Excel, no deberías guardar el workbook en formato Excel más adelante. De lo contrario, podría producirse un error inesperado en el archivo Excel generado.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignora los datos que no se imprimen al imprimir directamente el archivo

**Remarks**

Solo para archivos xlsx.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.

**Remarks**

Para escenarios en los que el usuario solo necesita leer algunos contenidos del archivo de plantilla y no necesita guardar el workbook, establecer esta propiedad como falsa puede mejorar el rendimiento, especialmente cuando se usa junto con algún tipo de LoadFilter.

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indica si solo se ajustan las filas cuya altura no está personalizada.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indica si se analiza la fórmula al leer el archivo.

**Remarks**

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm y Xlsm porque las fórmulas en los archivos se almacenan como una cadena de fórmula.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es falso.

**Remarks**

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm, Xlsm y xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Obtiene la contraseña del libro de trabajo.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Después de cargar el libro de trabajo desde un archivo de plantilla con esta opción, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) se establecerá al mismo valor que esta propiedad.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indica si se filtra automáticamente los datos al cargar los archivos.

**Remarks**

A veces, aunque el autofiltro está configurado, las filas correspondientes no se ocultan en el archivo. Ahora solo funciona para archivos SpreadSheetML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Comprueba si los datos son válidos en el archivo de plantilla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si la propiedad es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que no es válido para el formato de archivo Excel, no deberías guardar el workbook en formato Excel más adelante. De lo contrario, podría producirse un error inesperado en el archivo Excel generado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignora los datos que no se imprimen al imprimir directamente el archivo

**Remarks**

Solo para archivos xlsx.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.

**Remarks**

Para escenarios en los que el usuario solo necesita leer algunos contenidos del archivo de plantilla y no necesita guardar el workbook, establecer esta propiedad como falsa puede mejorar el rendimiento, especialmente cuando se usa junto con algún tipo de LoadFilter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indica si solo se ajustan las filas cuya altura no está personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indica si se analiza la fórmula al leer el archivo.

**Remarks**

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm y Xlsm porque las fórmulas en los archivos se almacenan como una cadena de fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es falso.

**Remarks**

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm, Xlsm y xlsb.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Establece la contraseña del workbook.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Después de cargar el libro de trabajo desde un archivo de plantilla con esta opción, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) se establecerá al mismo valor que esta propiedad.

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

