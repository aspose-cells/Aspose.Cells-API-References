---
title: "GridTxtLoadOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para cargar un archivo de texto."
type: docs
url: /es/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Representa las opciones para cargar un archivo de texto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Crea las opciones para cargar un archivo de texto. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [getCheckDataValid()](#getCheckDataValid--) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos de fecha. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos numéricos. |
| [getEncoding()](#getEncoding--) | Obtiene la codificación predeterminada. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Indica si los datos se extienden a la hoja siguiente cuando las filas o columnas de datos superan el límite. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [getKeepPrecision()](#getKeepPrecision--) | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [getOnlyAuto()](#getOnlyAuto--) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica si se analiza la fórmula al leer el archivo. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [getPassword()](#getPassword--) | Obtiene la contraseña del libro de trabajo. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [getSeparator()](#getSeparator--) | Obtiene el separador de caracteres del archivo de texto. |
| [getSeparatorString()](#getSeparatorString--) | Obtiene un valor de cadena como separador. |
| [getTextQualifier()](#getTextQualifier--) | Especifica el calificador de texto para los valores de celda. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Indica si los delimitadores consecutivos deben tratarse como uno solo. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. |
| [hasFormula()](#hasFormula--) | Indica si el texto es una fórmula si comienza con "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Indica si hay calificador de texto para el valor de la celda. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Verdadero significa que el archivo contiene varias codificaciones. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Establece la codificación predeterminada. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Indica si los datos se extienden a la hoja siguiente cuando las filas o columnas de datos superan el límite. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indica si el texto es una fórmula si comienza con "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Indica si hay calificador de texto para el valor de la celda. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Verdadero significa que el archivo contiene varias codificaciones. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica si se analiza la fórmula al leer el archivo. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Establece la contraseña del workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [setSeparator(char value)](#setSeparator-char-) | Establece el separador de caracteres del archivo de texto. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Establece un valor de cadena como separador. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Especifica el calificador de texto para los valores de celda. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Indica si los delimitadores consecutivos deben tratarse como uno solo. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Crea las opciones para cargar un archivo de texto.

**Remarks**

El tipo de archivo de carga predeterminado es CSV.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos de fecha.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos numéricos.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtiene la codificación predeterminada. Solo se aplica a archivos csv.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Si extiende los datos a la hoja siguiente cuando las filas o columnas de datos superan el límite. Si esta propiedad es verdadera, los datos adicionales se extenderán a la hoja siguiente detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro actual). Si esta propiedad es falsa, los datos que superen el límite se ignorarán. El valor predeterminado es falso;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignora los datos que no se imprimen al imprimir directamente el archivo

**Remarks**

Solo para archivos xlsx.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indica si no se analiza un valor de cadena cuando la longitud es 15.

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Obtiene el separador de caracteres del archivo de texto.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Obtiene un valor de cadena como separador.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'.

**Remarks**

Al establecer esta propiedad, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) se volverá verdadera automáticamente.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Indica si los delimitadores consecutivos deben tratarse como uno solo.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) se establecerá como verdadero para la celda.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indica si el texto es una fórmula si comienza con "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es verdadero.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Verdadero significa que el archivo contiene varias codificaciones.

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Establece la codificación predeterminada. Sólo se aplica a archivos csv.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Si extiende los datos a la hoja siguiente cuando las filas o columnas de datos superan el límite. Si esta propiedad es verdadera, los datos adicionales se extenderán a la hoja siguiente detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro actual). Si esta propiedad es falsa, los datos que superen el límite se ignorarán. El valor predeterminado es falso;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indica si el texto es una fórmula si comienza con "=".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es verdadero.

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indica si no se analiza un valor de cadena cuando la longitud es 15.

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Verdadero significa que el archivo contiene varias codificaciones.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Establece el separador de caracteres del archivo de texto.

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

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'.

**Remarks**

Al establecer esta propiedad, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) se volverá verdadera automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Indica si los delimitadores consecutivos deben tratarse como uno solo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) se establecerá como verdadero para la celda.

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

