---
title: "TxtLoadOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones para cargar un archivo de texto."
type: docs
url: /es/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Representa las opciones para cargar un archivo de texto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Crea las opciones para cargar un archivo de texto. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Crea las opciones para cargar un archivo de texto. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Obtiene las opciones del ajuste automático |
| [getCheckDataValid()](#getCheckDataValid--) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos de fecha. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtiene un valor que indica si la cadena en el archivo de texto se convierte a datos numéricos. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo |
| [getEncoding()](#getEncoding--) | Obtiene la codificación predeterminada. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Indica si los datos se extienden a la hoja siguiente cuando las filas o columnas de datos superan el límite. |
| [getFontConfigs()](#getFontConfigs--) | Obtiene la configuración individual de fuentes. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | El número de columnas de encabezado que se repetirán para hojas extendidas. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | El número de filas de encabezado que se repetirán para hojas extendidas. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indica si se ignoran formas inútiles. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Obtiene el monitor de interrupciones. |
| [getKeepPrecision()](#getKeepPrecision--) | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [getLanguageCode()](#getLanguageCode--) | Obtiene el idioma de la interfaz de usuario de la versión del Libro de trabajo basado en el CountryCode con el que se guardó el archivo. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla. |
| [getLoadFilter()](#getLoadFilter--) | El filtro que indica cómo cargar los datos. |
| [getLoadFormat()](#getLoadFormat--) | Obtiene el formato de carga. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha y hora. |
| [getLocale()](#getLocale--) | Obtiene la configuración regional utilizada para el Libro de trabajo que se cargará. |
| [getMaxColumnCount()](#getMaxColumnCount--) | El número máximo de columnas que se importarán para una hoja. |
| [getMaxRowCount()](#getMaxRowCount--) | El número máximo de filas que se pueden importar para una hoja. |
| [getMemorySetting()](#getMemorySetting--) | Obtiene el modo de memoria para el libro de trabajo cargado. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica si se analiza la fórmula al leer el archivo. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [getPassword()](#getPassword--) | Obtiene la contraseña del libro de trabajo. |
| [getPreferredParsers()](#getPreferredParsers--) | Obtiene los analizadores de valores preferidos para cargar el archivo de texto. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [getRegion()](#getRegion--) | Obtiene la configuración regional utilizada para el Libro de trabajo que se cargará. |
| [getSeparator()](#getSeparator--) | Obtiene el separador de caracteres del archivo de texto. |
| [getSeparatorString()](#getSeparatorString--) | Obtiene un valor de cadena como separador. |
| [getStandardFont()](#getStandardFont--) | Establece el nombre de fuente estándar predeterminado |
| [getStandardFontSize()](#getStandardFontSize--) | Establece el tamaño de fuente estándar predeterminado. |
| [getTextQualifier()](#getTextQualifier--) | Especifica el calificador de texto para los valores de celda. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Indica si los delimitadores consecutivos deben tratarse como uno solo. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hasFormula()](#hasFormula--) | Indica si el texto es una fórmula si comienza con "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Indica si hay calificador de texto para el valor de la celda. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Verdadero significa que el archivo contiene varias codificaciones. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Establece las opciones del ajuste automático |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Comprueba si los datos son válidos en el archivo de plantilla. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Establece la codificación predeterminada. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Indica si los datos se extienden a la hoja siguiente cuando las filas o columnas de datos superan el límite. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Establece configuraciones individuales de fuentes. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indica si el texto es una fórmula si comienza con "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Indica si hay calificador de texto para el valor de la celda. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | El número de columnas de encabezado que se repetirán para hojas extendidas. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | El número de filas de encabezado que se repetirán para hojas extendidas. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indica si se ignoran formas inútiles. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Establece el monitor de interrupciones. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica si se mantiene los datos no analizados en memoria para el Libro de trabajo cuando se carga desde un archivo de plantilla. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Establece el idioma de la interfaz de usuario de la versión del Workbook según el CountryCode con el que se guardó el archivo. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | El filtro que indica cómo cargar los datos. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha y hora. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Establece la configuración regional utilizada para el Workbook que se cargará. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | El número máximo de columnas que se importarán para una hoja. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | El número máximo de filas que se pueden importar para una hoja. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Establece el modo de memoria para el workbook cargado. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Verdadero significa que el archivo contiene varias codificaciones. |
| [setPaperSize(int type)](#setPaperSize-int-) | Establece el tamaño de papel de impresión predeterminado según la configuración de la impresora predeterminada. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica si se analiza la fórmula al leer el archivo. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Establece la contraseña del workbook. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Establece los analizadores de valores preferidos para cargar el archivo de texto. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [setRegion(int value)](#setRegion-int-) | Establece la configuración regional utilizada para el Workbook que se cargará. |
| [setSeparator(char value)](#setSeparator-char-) | Establece el separador de caracteres del archivo de texto. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Establece un valor de cadena como separador. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Establece el nombre de fuente estándar predeterminado |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Establece el tamaño de fuente estándar predeterminado. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Especifica el calificador de texto para los valores de celda. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Indica si los delimitadores consecutivos deben tratarse como uno solo. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Crea las opciones para cargar un archivo de texto.

**Remarks**

El tipo de archivo de carga predeterminado es CSV.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Crea las opciones para cargar un archivo de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). El formato de carga |

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
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Obtiene las opciones del ajuste automático

**Remarks**

Solo para archivos xlsx, spreadsheetML por ahora.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
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


Obtiene un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtiene un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtiene la codificación predeterminada. Solo se aplica a archivos csv.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Indica si se extienden los datos a la hoja siguiente cuando las filas o columnas de datos superan el límite. El valor predeterminado es falso.

**Remarks**

Si esta propiedad es verdadera, los datos adicionales se colocarán en la hoja siguiente detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro de trabajo). Si esta propiedad es falsa, los datos que superen el límite se ignorarán.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Obtiene configuraciones individuales de fuentes. Solo funciona para el [Workbook](../../com.aspose.cells/workbook) que utiliza estas [LoadOptions](../../com.aspose.cells/loadoptions) para cargar.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


El número de columnas de encabezado que se repetirán para hojas extendidas.

**Remarks**

Las columnas de encabezado especificadas por esta propiedad se duplicarán en esas hojas extendidas. Esta propiedad solo tiene efecto cuando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) es verdadera.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


El número de filas de encabezado que se repetirán para hojas extendidas.

**Remarks**

Las filas de encabezado especificadas por esta propiedad se duplicarán en esas hojas extendidas. Esta propiedad solo tiene efecto cuando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) es verdadera.

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignora los datos que no se imprimen al imprimir directamente el archivo

**Remarks**

Solo para archivos xlsx.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Indica si se ignoran formas inútiles.

**Remarks**

Solo funciona para archivos xlsx, xlsb y xlsm. Hay muchas formas idénticas superpuestas que son inútiles en algunos archivos; podemos ignorarlas al cargar los archivos.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Obtiene el monitor de interrupciones.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
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
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Obtiene el idioma de la interfaz de usuario de la versión del Libro de trabajo basado en el CountryCode con el que se guardó el archivo.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


El filtro que indica cómo cargar los datos.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Obtiene el formato de carga.

Ver [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha y hora.

Vea [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Obtiene la configuración regional utilizada para el Libro de trabajo que se cargará.

**Remarks**

Esta propiedad tiene el mismo efecto que [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) para establecer la configuración regional.

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


El número máximo de columnas que se importarán para una hoja.

**Remarks**

Las columnas que superen este límite se ignorarán o se extenderán a la hoja siguiente según [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Este recuento incluye las columnas de encabezado([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). El valor máximo es el límite de columnas del formato de archivo correspondiente, por ejemplo, para archivos xlsx es 16384. Si esta propiedad no se ha especificado o el valor especificado no es positivo, se utilizará también el límite máximo.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


El número máximo de filas que se pueden importar para una hoja.

**Remarks**

Las filas que superen este límite se ignorarán o se extenderán a la hoja siguiente según [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Este recuento incluye las filas de encabezado([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). El valor máximo permitido es el límite de filas del formato de archivo correspondiente, por ejemplo, para archivos xlsx es 1048576. Si esta propiedad no se ha especificado o el valor especificado no es positivo, se utilizará también el límite máximo.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Obtiene el modo de memoria para el libro de trabajo cargado.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Para más detalles sobre el modo de memoria, consulte [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
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
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Obtiene los analizadores de valores preferidos para cargar el archivo de texto.

**Remarks**

parsers[0] es el analizador que se usará para la primera columna en el archivo de plantilla de texto, parsers[1] es el analizador que se usará para la segunda columna, ...etc. El último (parsers[parsers.length-1]) se usará para todas las demás columnas a partir de parsers.length-1. Si un elemento es nulo, la columna correspondiente será analizada por el analizador predeterminado de Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Después de cargar el libro de trabajo desde un archivo de plantilla con esta opción, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) se establecerá al mismo valor que esta propiedad.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Obtiene la configuración regional utilizada para el Libro de trabajo que se cargará.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

La configuración regional puede usarse para inicializar algunas funciones del libro de trabajo, como fuentes, temas, etc. Para formatos de archivo basados en texto, como CSV, HTML, ..., la configuración regional también se utilizará para detectar formatos numéricos y analizar valores de texto a valores numéricos o de fecha y hora para las celdas. Esta configuración se mantendrá para el libro de trabajo instanciado posteriormente, es decir, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) del libro de trabajo utilizará la misma región que esta propiedad.

**Returns:**
int
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
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Establece el nombre de fuente estándar predeterminado

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Establece el tamaño de fuente estándar predeterminado.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'.

**Remarks**

Al establecer esta propiedad, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) se volverá verdadera automáticamente.

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


Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) se establecerá como verdadero para la celda.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtiene la devolución de llamada de advertencia.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Establece las opciones del ajuste automático

**Remarks**

Solo para archivos xlsx, spreadsheetML por ahora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

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


Establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Establece la codificación predeterminada. Sólo se aplica a archivos csv.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Indica si se extienden los datos a la hoja siguiente cuando las filas o columnas de datos superan el límite. El valor predeterminado es falso.

**Remarks**

Si esta propiedad es verdadera, los datos adicionales se colocarán en la hoja siguiente detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro de trabajo). Si esta propiedad es falsa, los datos que superen el límite se ignorarán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Establece configuraciones de fuentes individuales. Solo funciona para el [Workbook](../../com.aspose.cells/workbook) que utiliza este [LoadOptions](../../com.aspose.cells/loadoptions) para cargar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


El número de columnas de encabezado que se repetirán para hojas extendidas.

**Remarks**

Las columnas de encabezado especificadas por esta propiedad se duplicarán en esas hojas extendidas. Esta propiedad solo tiene efecto cuando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) es verdadera.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


El número de filas de encabezado que se repetirán para hojas extendidas.

**Remarks**

Las filas de encabezado especificadas por esta propiedad se duplicarán en esas hojas extendidas. Esta propiedad solo tiene efecto cuando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) es verdadera.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Indica si se ignoran formas inútiles.

**Remarks**

Solo funciona para archivos xlsx, xlsb y xlsm. Hay muchas formas idénticas superpuestas que son inútiles en algunos archivos; podemos ignorarlas al cargar los archivos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Establece el monitor de interrupciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

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

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Establece el idioma de la interfaz de usuario de la versión del Workbook según el CountryCode con el que se guardó el archivo.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


El filtro que indica cómo cargar los datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha y hora.

Vea [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Establece la configuración regional utilizada para el Workbook que se cargará.

**Remarks**

Esta propiedad tiene el mismo efecto que [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) para establecer la configuración regional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


El número máximo de columnas que se importarán para una hoja.

**Remarks**

Las columnas que superen este límite se ignorarán o se extenderán a la hoja siguiente según [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Este recuento incluye las columnas de encabezado([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). El valor máximo es el límite de columnas del formato de archivo correspondiente, por ejemplo, para archivos xlsx es 16384. Si esta propiedad no se ha especificado o el valor especificado no es positivo, se utilizará también el límite máximo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


El número máximo de filas que se pueden importar para una hoja.

**Remarks**

Las filas que superen este límite se ignorarán o se extenderán a la hoja siguiente según [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Este recuento incluye las filas de encabezado([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). El valor máximo permitido es el límite de filas del formato de archivo correspondiente, por ejemplo, para archivos xlsx es 1048576. Si esta propiedad no se ha especificado o el valor especificado no es positivo, se utilizará también el límite máximo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Establece el modo de memoria para el workbook cargado.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Para más detalles sobre el modo de memoria, consulte [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Verdadero significa que el archivo contiene varias codificaciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Establece el tamaño de papel de impresión predeterminado según la configuración de la impresora predeterminada.

**Remarks**

Si no hay una configuración sobre el tamaño del papel, MS Excel usará la configuración predeterminada de la impresora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). El tamaño de papel predeterminado. |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Establece los analizadores de valores preferidos para cargar el archivo de texto.

**Remarks**

parsers[0] es el analizador que se usará para la primera columna en el archivo de plantilla de texto, parsers[1] es el analizador que se usará para la segunda columna, ...etc. El último (parsers[parsers.length-1]) se usará para todas las demás columnas a partir de parsers.length-1. Si un elemento es nulo, la columna correspondiente será analizada por el analizador predeterminado de Aspose.Cells.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Después de cargar el libro de trabajo desde un archivo de plantilla con esta opción, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) se establecerá al mismo valor que esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Establece la configuración regional utilizada para el Workbook que se cargará.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

La configuración regional puede usarse para inicializar algunas funciones del libro de trabajo, como fuentes, temas, etc. Para formatos de archivo basados en texto, como CSV, HTML, ..., la configuración regional también se utilizará para detectar formatos numéricos y analizar valores de texto a valores numéricos o de fecha y hora para las celdas. Esta configuración se mantendrá para el libro de trabajo instanciado posteriormente, es decir, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) del libro de trabajo utilizará la misma región que esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Establece el nombre de fuente estándar predeterminado

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Establece el tamaño de fuente estándar predeterminado.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'.

**Remarks**

Al establecer esta propiedad, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) se volverá verdadera automáticamente.

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


Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es verdadero. Si es falso, la comilla simple inicial se eliminará del valor de la celda correspondiente y [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) se establecerá como verdadero para la celda.

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

