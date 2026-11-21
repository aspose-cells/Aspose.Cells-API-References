---
title: "CellsHelper"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Proporciona funciones auxiliares."
type: docs
url: /es/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Proporciona funciones auxiliares.
## Métodos

| Método | Descripción |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Agregar función de complemento. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Obtiene los índices de fila y columna de la celda según su nombre. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Obtiene el nombre de la columna según el índice de columna. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Obtiene el índice de columna según el nombre de la columna. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Convierte la fórmula A1 de la celda a la fórmula r1c1. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Convierte la fórmula r1c1 de la celda a la fórmula A1. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Obtiene la ruta de inicio alternativa, a la que hacen referencia algunas referencias de fórmulas externas. |
| [getCacheFolder()](#getCacheFolder--) | Obtiene la carpeta para archivos temporales que pueden usarse como caché de datos. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Obtiene la fábrica para crear instancias con implementación especial. |
| [getDPI()](#getDPI--) | Obtiene los DPI de la máquina. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Convierte el valor double al valor de fecha y hora. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Convierte la fecha y hora a un valor double. |
| [getLibraryPath()](#getLibraryPath--) | Obtiene la ruta de la biblioteca a la que hacen referencia algunas referencias de fórmulas externas. |
| [getSignificantDigits()](#getSignificantDigits--) | Obtiene el número de dígitos significativos. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Obtiene el tipo predeterminado de dígitos significativos para la salida de valores numéricos. |
| [getStartupPath()](#getStartupPath--) | Obtiene la ruta de inicio, a la que hacen referencia algunas referencias de fórmulas externas. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Obtiene el ancho del texto en unidades de puntos. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Obtiene todos los colores usados en el libro de trabajo. |
| [getVersion()](#getVersion--) | Obtiene la versión de lanzamiento. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Establezca esta propiedad en True cuando se ejecute en una plataforma en la nube, como: Azure, AWSLambda, etc, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Fusiona algunos archivos xls grandes en un archivo xls. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Indica si el nombre de la hoja debe estar entre comillas simples. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Obtiene el nombre de fila según el índice de fila. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Obtiene el índice de fila según el nombre de fila. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Establece la ruta de inicio alternativa, a la que hacen referencia algunas referencias de fórmulas externas. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Establece la carpeta para archivos temporales que pueden usarse como caché de datos. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Establezca esta propiedad en True cuando se ejecute en una plataforma en la nube, como: Azure, AWSLambda, etc, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Establece la fábrica para crear instancias con una implementación especial. |
| [setDPI(double value)](#setDPI-double-) | Obtiene los DPI de la máquina. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Establece la ruta de la biblioteca a la que se hace referencia en algunas referencias de fórmulas externas. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Establece el número de dígitos significativos. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Establece el tipo predeterminado de dígitos significativos para la salida de valores numéricos. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Establece la ruta de inicio, a la que se hace referencia en algunas referencias de fórmulas externas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Agregar función de complemento.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice los métodos WorksheetCollection.RegisterAddInFunction(). Este método será eliminado 12 meses después, desde enero de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| función | java.lang.String | El nombre de la función. |
| minCountOfParameters | int | Número mínimo de parámetros que requiere esta función |
| maxCountOfParameters | int | Número máximo de parámetros que permite esta función. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). El tipo de parámetros esperado de la función |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). El tipo de valor de la función. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Obtiene el nombre de la celda según sus índices de fila y columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |

**Returns:**
java.lang.String - Nombre de la celda.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Obtiene los índices de fila y columna de la celda según su nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de la celda |

**Returns:**
int[] - [0] es el índice de fila y [1] es el índice de columna.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Obtiene el nombre de la columna según el índice de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

**Returns:**
java.lang.String - Nombre de la columna.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Obtiene el índice de columna según el nombre de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnName | java.lang.String | Nombre de columna. |

**Returns:**
int - Índice de columna.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Convierte la fórmula A1 de la celda a la fórmula r1c1.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Worksheet.ConvertFormulaReferenceStyle(). Esta propiedad será eliminada 12 meses después, desde agosto de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula A1. |
| fila | int | El índice de fila de la celda. |
| columna | int | El índice de columna de la celda. |

**Returns:**
java.lang.String - La fórmula R1C1.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Convierte la fórmula r1c1 de la celda a la fórmula A1.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Worksheet.ConvertFormulaReferenceStyle(). Esta propiedad será eliminada 12 meses después, desde agosto de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| r1c1Formula | java.lang.String | La fórmula r1c1. |
| fila | int | El índice de fila de la celda. |
| columna | int | El índice de columna de la celda. |

**Returns:**
java.lang.String - La fórmula A1.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Comprueba el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por ' ', luego se devolverá el valor de cadena reconstruido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nameProposal | java.lang.String | nombre de hoja a usar |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Comprueba el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por el carácter especificado, luego se devolverá el valor de cadena reconstruido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nameProposal | java.lang.String | nombre de hoja a usar |
| replaceChar | char | carácter que se utilizará para reemplazar los caracteres no válidos en el nombre de hoja proporcionado |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Obtiene la ruta de inicio alternativa, a la que hacen referencia algunas referencias de fórmulas externas.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Obtiene la carpeta para archivos temporales que pueden usarse como caché de datos.

**Remarks**

Los archivos de caché se utilizan generalmente para algunas funciones relacionadas con el rendimiento de la memoria, como guardar conjuntos de datos grandes en un archivo xls, o usar el modo de memoria con caché de archivos para el modelo de celdas.

**Returns:**
java.lang.String - Carpeta para los archivos de caché que se ha especificado. Si no se ha especificado, se devolverá null y se utilizará la ruta temporal del sistema cuando sea necesario.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Obtiene la fábrica para crear instancias con implementación especial.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Obtiene los DPI de la máquina.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Convierte el valor double al valor de fecha y hora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleValue | double | El valor double. |
| date1904 | boolean | Sistema de fecha 1904. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Convierte la fecha y hora a un valor double.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora. |
| date1904 | boolean | Sistema de fecha 1904. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Obtiene la ruta de la biblioteca a la que hacen referencia algunas referencias de fórmulas externas.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Obtiene el número de dígitos significativos. El valor predeterminado es 17.

**Remarks**

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Esta propiedad será eliminada 12 meses después, a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Obtiene el tipo predeterminado de dígitos significativos para la salida de valores numéricos. El valor predeterminado es [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Ver [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Obtiene la ruta de inicio, a la que hacen referencia algunas referencias de fórmulas externas.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Obtiene el ancho del texto en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | El texto. |
| font | [Font](../../com.aspose.cells/font) | La fuente del texto. |
| escalado | double | El escalado del texto. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Obtiene todos los colores usados en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | El objeto del libro de trabajo. |

**Returns:**
com.aspose.cells.Color[] - Los colores utilizados.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Obtiene la versión de lanzamiento.

**Returns:**
java.lang.String - La versión de lanzamiento.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Establezca esta propiedad en True cuando se ejecute en una plataforma en la nube, como: Azure, AWSLambda, etc,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Fusiona algunos archivos xls grandes en un archivo xls.

**Remarks**

Este método solo admite la fusión de datos, estilo y fórmulas al nuevo archivo. El archivo en caché se utiliza para almacenar algunos datos temporales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivos | java.lang.String[] | Los archivos. |
| cachedFile | java.lang.String | El archivo en caché. |
| destFile | java.lang.String | El archivo dest. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Indica si el nombre de la hoja debe estar entre comillas simples.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | El nombre de la hoja |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Obtiene el nombre de fila según el índice de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

**Returns:**
java.lang.String - Nombre de la fila.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Obtiene el índice de fila según el nombre de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowName | java.lang.String | Nombre de fila. |

**Returns:**
int - Índice de fila.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Establece la ruta de inicio alternativa, a la que hacen referencia algunas referencias de fórmulas externas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Establece la carpeta para archivos temporales que pueden usarse como caché de datos.

**Remarks**

Los archivos de caché se utilizan generalmente para algunas funciones relacionadas con el rendimiento de la memoria, como guardar conjuntos de datos grandes en un archivo xls, o usar el modo de memoria con caché de archivos para el modelo de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| caché | java.lang.String | Carpeta para archivos temporales que pueden usarse como caché de datos. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Establezca esta propiedad en True cuando se ejecute en una plataforma en la nube, como: Azure, AWSLambda, etc,

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Establece la fábrica para crear instancias con una implementación especial.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Obtiene los DPI de la máquina.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Establece la ruta de la biblioteca a la que se hace referencia en algunas referencias de fórmulas externas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Establece el número de dígitos significativos. El valor predeterminado es 17.

**Remarks**

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Esta propiedad será eliminada 12 meses después, a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Establece el tipo predeterminado de dígitos significativos para la salida de valores numéricos. El valor predeterminado es [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Ver [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Establece la ruta de inicio, a la que se hace referencia en algunas referencias de fórmulas externas.

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

