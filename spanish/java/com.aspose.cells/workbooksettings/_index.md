---
title: "WorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las configuraciones del libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Representa todas las configuraciones del libro de trabajo.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Métodos

| Método | Descripción |
| --- | --- |
| [dispose()](#dispose--) | Libera recursos. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtiene el autor del archivo. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Especifica un valor booleano que indica que la aplicación comprimió automáticamente las imágenes en el libro de trabajo. |
| [getAutoRecover()](#getAutoRecover--) | Indica si el archivo está marcado para recuperación automática. |
| [getBuildVersion()](#getBuildVersion--) | Especifica la versión pública incremental de la aplicación. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro de trabajo. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indica si se verifica el formato numérico personalizado al establecer Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Especifica la versión OOXML para el documento de salida. |
| [getCrashSave()](#getCrashSave--) | Indica si la aplicación guardó por última vez el archivo del libro de trabajo después de un bloqueo. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Indica si la aplicación abrió por última vez el libro de trabajo para recuperación de datos. |
| [getDate1904()](#getDate1904--) | Obtiene un valor que representa si el libro de trabajo usa el sistema de fechas 1904. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Obtiene la resolución predeterminada de la imagen. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Obtiene la configuración de los valores predeterminados de las propiedades relacionadas con el estilo para este libro de trabajo. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Indica si se descarta la edición de datos de imagen. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Indica si y cómo mostrar objetos en el libro de trabajo. |
| [getEnableMacros()](#getEnableMacros--) | Habilitar macros; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Obtiene la primera pestaña de hoja de cálculo visible. |
| [getFormulaSettings()](#getFormulaSettings--) | Obtiene la configuración de las funciones relacionadas con fórmulas. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Obtiene la configuración de globalización. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Obtiene si se oculta la lista de campos para la tabla dinámica. |
| [getLanguageCode()](#getLanguageCode--) | Obtiene el idioma de la interfaz de usuario de la versión del Libro de trabajo basado en el CountryCode con el que se guardó el archivo. |
| [getLocale()](#getLocale--) | Obtiene la configuración regional usada por este libro de trabajo. |
| [getMaxColumn()](#getMaxColumn--) | Obtiene el índice máximo de columna, basado en cero. |
| [getMaxRow()](#getMaxRow--) | Obtiene el índice máximo de fila, basado en cero. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Obtiene el número máximo de fila de la fórmula compartida. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Obtiene la limitación de elementos únicos por campo |
| [getMemorySetting()](#getMemorySetting--) | Obtiene las opciones de uso de memoria. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Obtiene el separador decimal para formatear/analizar valores numéricos. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Obtiene el carácter que separa grupos de dígitos a la izquierda del decimal en valores numéricos. |
| [getPaperSize()](#getPaperSize--) | Obtiene el tamaño de papel de impresión predeterminado. |
| [getPassword()](#getPassword--) | Representa la contraseña de cifrado del archivo Workbook. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia. |
| [getProtectionType()](#getProtectionType--) | Obtiene el tipo de protección del workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Indica si al establecer la propiedad [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda |
| [getRegion()](#getRegion--) | Obtiene la configuración regional del workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Verdadero si la información personal puede eliminarse del workbook especificado. |
| [getRepairLoad()](#getRepairLoad--) | Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación. |
| [getResourceProvider()](#getResourceProvider--) | Obtiene el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Obtiene cómo la aplicación muestra las formas en este workbook |
| [getShared()](#getShared--) | Obtiene un valor que indica si el Workbook está compartido. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana). |
| [getShowTabs()](#getShowTabs--) | Obtiene un valor que indica si se muestran las pestañas del Workbook. |
| [getSignificantDigits()](#getSignificantDigits--) | Obtiene el número de dígitos significativos. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Obtiene el tipo de dígitos significativos para la salida de valores numéricos en este workbook. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Obtiene las opciones de la etiqueta inteligente. |
| [getStreamProvider()](#getStreamProvider--) | Obtiene el proveedor de flujo para recursos externos. |
| [getThemeFont(int type)](#getThemeFont-int-) | Obtiene el nombre de fuente predeterminada del tema. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Indica si se actualiza el borde de las celdas adyacentes. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Obtiene cómo se actualizan los enlaces externos cuando se abre el workbook. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [getWindowHeight()](#getWindowHeight--) | La altura de la ventana, en unidades de punto. |
| [getWindowHeightCM()](#getWindowHeightCM--) | La altura de la ventana, en unidades de centímetro. |
| [getWindowHeightInch()](#getWindowHeightInch--) | La altura de la ventana, en unidad de pulgada. |
| [getWindowLeft()](#getWindowLeft--) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidad de punto. |
| [getWindowLeftCM()](#getWindowLeftCM--) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. |
| [getWindowLeftInch()](#getWindowLeftInch--) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. |
| [getWindowTop()](#getWindowTop--) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de punto. |
| [getWindowTopCM()](#getWindowTopCM--) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de centímetro. |
| [getWindowTopInch()](#getWindowTopInch--) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de pulgada. |
| [getWindowWidth()](#getWindowWidth--) | El ancho de la ventana, en unidad de punto. |
| [getWindowWidthCM()](#getWindowWidthCM--) | El ancho de la ventana, en unidad de centímetro. |
| [getWindowWidthInch()](#getWindowWidthInch--) | El ancho de la ventana, en unidad de pulgada. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indica si debe ser compatible con WPS. |
| [getWriteProtection()](#getWriteProtection--) | Proporciona acceso a las opciones de protección de escritura del libro de trabajo. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Indica si se cifra el libro de trabajo con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas. |
| [isEncrypted()](#isEncrypted--) | Obtiene un valor que indica si se requiere una contraseña para abrir este libro de trabajo. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Obtiene un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal. |
| [isHidden()](#isHidden--) | Indica si este libro de trabajo está oculto. |
| [isMinimized()](#isMinimized--) | Representa si la hoja de cálculo generada se abrirá minimizada. |
| [isProtected()](#isProtected--) | Obtiene un valor que indica si la estructura o la ventana del libro de trabajo está protegida. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Obtiene un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece el autor del archivo. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Especifica un valor booleano que indica que la aplicación comprimió automáticamente las imágenes en el libro de trabajo. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Indica si el archivo está marcado para recuperación automática. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Especifica la versión pública incremental de la aplicación. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro de trabajo. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indica si se verifica el formato numérico personalizado al establecer Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setCompliance(int value)](#setCompliance-int-) | Especifica la versión OOXML para el documento de salida. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Indica si la aplicación guardó por última vez el archivo del libro de trabajo después de un bloqueo. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Indica si la aplicación abrió por última vez el libro de trabajo para recuperación de datos. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Establece un valor que representa si el libro de trabajo usa el sistema de fechas 1904. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Indica si se cifra el libro de trabajo con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Establece la resolución predeterminada de la imagen. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Indica si se descarta la edición de datos de imagen. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Indica si y cómo mostrar objetos en el libro de trabajo. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Habilitar macros; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Establece la primera pestaña de hoja de cálculo visible. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Establece la configuración de globalización. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica si este libro de trabajo está oculto. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Establece si ocultar la lista de campos para la tabla dinámica. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Establece el idioma de la interfaz de usuario de la versión del Workbook según el CountryCode con el que se guardó el archivo. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Establece el Locale utilizado por este libro de trabajo. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Establece el número máximo de filas de la fórmula compartida. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Establece la limitación de elementos únicos por campo. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Establece las opciones de uso de memoria. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Representa si la hoja de cálculo generada se abrirá minimizada. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Establece el separador decimal para formatear/analizar valores numéricos. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Establece el carácter que separa los grupos de dígitos a la izquierda del decimal en valores numéricos. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Establece el tipo de orientación de impresión para todo el libro de trabajo. |
| [setPaperSize(int value)](#setPaperSize-int-) | Establece el tamaño de papel de impresión predeterminado. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Representa la contraseña de cifrado del archivo Workbook. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Indica si al establecer la propiedad [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda |
| [setRegion(int value)](#setRegion-int-) | Establece la configuración regional para el libro de trabajo. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Verdadero si la información personal puede eliminarse del workbook especificado. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Establece el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Establece cómo la aplicación muestra las formas en este libro de trabajo. |
| [setShared(boolean value)](#setShared-boolean-) | Establece un valor que indica si el libro de trabajo está compartido. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Establece un valor que indica si se muestran las pestañas del libro de trabajo. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Establece el número de dígitos significativos. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Establece el tipo de dígitos significativos para la salida de valores numéricos en este libro de trabajo. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Establece el proveedor de flujo para recursos externos. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Indica si se actualiza el borde de las celdas adyacentes. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Establece cómo se actualizan los enlaces externos cuando se abre el libro de trabajo. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | La altura de la ventana, en unidades de punto. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | La altura de la ventana, en unidades de centímetro. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | La altura de la ventana, en unidad de pulgada. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidad de punto. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. |
| [setWindowTop(double value)](#setWindowTop-double-) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de punto. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de centímetro. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de pulgada. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | El ancho de la ventana, en unidad de punto. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | El ancho de la ventana, en unidad de centímetro. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | El ancho de la ventana, en unidad de pulgada. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indica si debe ser compatible con WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Libera recursos.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtiene el autor del archivo.

**Remarks**

No está configurado, verifica primero [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--), luego verifica el usuario del Entorno.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Especifica un valor booleano que indica que la aplicación comprimió automáticamente las imágenes en el libro de trabajo.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Indica si el archivo está marcado para recuperación automática.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Especifica la versión pública incremental de la aplicación.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro de trabajo.

**Remarks**

El valor predeterminado es true. Solo para archivos xls o xlt de Excel97-2003.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indica si se verifica el formato numérico personalizado al establecer Style.Custom.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Especifica la versión OOXML para el documento de salida. El valor predeterminado es Ecma376\\_2006.

Ver [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Solo para archivos .xlsx.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Indica si la aplicación guardó por última vez el archivo del libro de trabajo después de un bloqueo.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Indica si la aplicación abrió por última vez el libro de trabajo para recuperación de datos.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtiene un valor que representa si el libro de trabajo usa el sistema de fechas 1904.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Obtiene la resolución predeterminada de la imagen.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Obtiene la configuración de los valores predeterminados de las propiedades relacionadas con el estilo para este libro de trabajo.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Indica si se descarta la edición de datos de imagen.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Indica si y cómo mostrar objetos en el libro de trabajo.

Ver [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Habilitar macros;

**Remarks**

Ahora solo funciona al copiar una hoja de cálculo a otra hoja de cálculo en un libro de trabajo.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Obtiene la primera pestaña de hoja de cálculo visible.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Obtiene la configuración de las funciones relacionadas con fórmulas.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Obtiene la configuración de globalización.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Obtiene si se oculta la lista de campos para la tabla dinámica.

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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Obtiene la configuración regional usada por este libro de trabajo.

**Remarks**

Devuelve null si ni Locale ni [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) están configurados.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Obtiene el índice máximo de columna, basado en cero.

**Remarks**

Devuelve 255 si el formato de archivo es Excel97-2003;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Obtiene el índice máximo de fila, basado en cero.

**Remarks**

Devuelve 65535 si el formato de archivo es Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Obtiene el número máximo de fila de la fórmula compartida.

**Remarks**

Si el número es demasiado grande, el autofiltro funciona muy lento en MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Obtiene la limitación de elementos únicos por campo

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Obtiene las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de cálculo recién creadas, pero no tendrá efecto en las hojas de cálculo existentes.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Para más detalles sobre el modo de memoria, consulte [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Obtiene el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Obtiene el carácter que separa los grupos de dígitos a la izquierda del decimal en valores numéricos. El predeterminado es el separador de grupos de la región actual.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Obtiene el tamaño de papel de impresión predeterminado.

Ver [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Si no hay una configuración sobre el tamaño del papel, MS Excel usará la configuración predeterminada de la impresora.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Representa la contraseña de cifrado del archivo Workbook.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Obtiene el tipo de protección del workbook.

Ver [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Indica si al establecer la propiedad [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Obtiene la configuración regional del workbook.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Configuración regional utilizada por el componente Aspose.Cells para un libro de trabajo cargado desde un archivo de plantilla: i). Para un archivo XLS, existen campos definidos para la configuración regional y MS Excel guarda los datos de configuración regional en el archivo al guardar el archivo XLS. Por lo tanto, utilizamos la región guardada en el archivo de plantilla para el libro de trabajo. Si no desea usar la región guardada en el archivo XLS, restáurela al valor esperado (por ejemplo, CountryCode.Default) después de cargar el archivo de plantilla. Además, guardamos el valor especificado por el usuario (mediante este método) en el archivo también al guardar un archivo XLS. ii). Para otros formatos de archivo, como XLSX, XLSB... etc., no hay un campo definido para la configuración regional en la especificación del formato de archivo. Por lo tanto, utilizamos la configuración regional del entorno de la aplicación para el libro de trabajo. Y el valor especificado por el usuario (mediante este método) no puede conservarse en los archivos generados con esos formatos. 2. Para el efecto de visualización en MS Excel: la configuración regional aplicada aquí solo puede tener efecto en tiempo de ejecución con el componente Aspose.Cells y no al visualizar el archivo generado con MS Excel. Incluso para el archivo XLS generado en el que se han guardado los datos de configuración regional especificados, al visualizar/editarlo con MS Excel, la región utilizada por MS Excel para formatear siempre es la configuración regional predeterminada del entorno donde se ejecuta MS Excel, no la que está guardada en el archivo. Es un comportamiento de MS Excel y no puede ser modificado por código.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Verdadero si la información personal puede eliminarse del workbook especificado.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Obtiene el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Obtiene cómo la aplicación muestra las formas en este workbook

Ver [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Obtiene un valor que indica si el Workbook está compartido.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Obtiene un valor que indica si se muestran las pestañas del Workbook.

**Remarks**

El valor predeterminado es true.

**Example**

El siguiente código oculta las pestañas de hoja y los botones de desplazamiento de pestañas para la hoja de cálculo.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Obtiene el número de dígitos significativos. El valor predeterminado es [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Esta propiedad será eliminada 12 meses después, a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Obtiene el tipo de dígitos significativos para la salida de valores numéricos en este libro de trabajo. El valor predeterminado es [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Ver [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Obtiene las opciones de la etiqueta inteligente.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtiene el proveedor de flujo para recursos externos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ResourceProvider. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Obtiene el nombre de fuente predeterminada del tema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). El tipo de esquema de la fuente. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Indica si se actualiza el borde de las celdas adyacentes.

**Remarks**

El valor predeterminado es false. Por ejemplo: el borde inferior de la celda A1 se actualiza, el borde superior de la celda A2 también debe cambiarse.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Obtiene cómo se actualizan los enlaces externos cuando se abre el workbook.

Ver [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtiene la devolución de llamada de advertencia.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


La altura de la ventana, en unidades de punto.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


La altura de la ventana, en unidades de centímetro.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


La altura de la ventana, en unidad de pulgada.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidad de punto.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de centímetros.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de pulgadas.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de punto.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de centímetro.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de pulgada.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


El ancho de la ventana, en unidad de punto.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


El ancho de la ventana, en unidad de centímetro.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


El ancho de la ventana, en unidad de pulgada.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indica si debe ser compatible con WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Proporciona acceso a las opciones de protección de escritura del libro de trabajo.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Indica si se cifra el libro de trabajo con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas.

**Remarks**

El valor predeterminado es false ahora. Es lo mismo que MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Obtiene un valor que indica si se requiere una contraseña para abrir este libro de trabajo.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Obtiene un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal.

**Remarks**

El valor predeterminado es true.

**Example**

El siguiente código hace que la barra de desplazamiento horizontal sea invisible para la hoja de cálculo.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica si este libro de trabajo está oculto.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Representa si la hoja de cálculo generada se abrirá minimizada.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Obtiene un valor que indica si la estructura o la ventana del libro de trabajo está protegida.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Obtiene un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical.

**Remarks**

El valor predeterminado es true.

**Example**

El siguiente código hace que la barra de desplazamiento vertical sea invisible para la hoja de cálculo.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Establece el autor del archivo.

**Remarks**

No está configurado, verifica primero [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--), luego verifica el usuario del Entorno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Especifica un valor booleano que indica que la aplicación comprimió automáticamente las imágenes en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Indica si el archivo está marcado para recuperación automática.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Especifica la versión pública incremental de la aplicación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro de trabajo.

**Remarks**

El valor predeterminado es true. Solo para archivos xls o xlt de Excel97-2003.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indica si se verifica el formato numérico personalizado al establecer Style.Custom.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Especifica la versión OOXML para el documento de salida. El valor predeterminado es Ecma376\\_2006.

Ver [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Solo para archivos .xlsx.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Indica si la aplicación guardó por última vez el archivo del libro de trabajo después de un bloqueo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Indica si la aplicación abrió por última vez el libro de trabajo para recuperación de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Establece un valor que representa si el libro de trabajo usa el sistema de fechas 1904.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Indica si se cifra el libro de trabajo con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas.

**Remarks**

El valor predeterminado es false ahora. Es lo mismo que MS Excel 2013.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Establece la resolución predeterminada de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Indica si se descarta la edición de datos de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Indica si y cómo mostrar objetos en el libro de trabajo.

Ver [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Habilitar macros;

**Remarks**

Ahora solo funciona al copiar una hoja de cálculo a otra hoja de cálculo en un libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Establece la primera pestaña de hoja de cálculo visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Establece la configuración de globalización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal.

**Remarks**

El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica si este libro de trabajo está oculto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Establece si ocultar la lista de campos para la tabla dinámica.

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

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Establece el Locale utilizado por este libro de trabajo.

**Remarks**

Devuelve null si ni Locale ni [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) están configurados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Establece el número máximo de filas de la fórmula compartida.

**Remarks**

Si el número es demasiado grande, el autofiltro funciona muy lento en MS Excel 2013.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Establece la limitación de elementos únicos por campo.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Establece las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de cálculo recién creadas, pero no tendrá efecto en las hojas de cálculo existentes.

Ver [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Para más detalles sobre el modo de memoria, consulte [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Representa si la hoja de cálculo generada se abrirá minimizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Establece el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Establece el carácter que separa los grupos de dígitos a la izquierda del decimal en valores numéricos. El predeterminado es el separador de grupos de la región actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Establece el tipo de orientación de impresión para todo el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). El tipo de orientación de página |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Establece el tamaño de papel de impresión predeterminado.

Ver [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Si no hay una configuración sobre el tamaño del papel, MS Excel usará la configuración predeterminada de la impresora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Representa la contraseña de cifrado del archivo Workbook.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Indica si al establecer la propiedad [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Establece la configuración regional para el libro de trabajo.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Configuración regional utilizada por el componente Aspose.Cells para un libro de trabajo cargado desde un archivo de plantilla: i). Para un archivo XLS, existen campos definidos para la configuración regional y MS Excel guarda los datos de configuración regional en el archivo al guardar el archivo XLS. Por lo tanto, utilizamos la región guardada en el archivo de plantilla para el libro de trabajo. Si no desea usar la región guardada en el archivo XLS, restáurela al valor esperado (por ejemplo, CountryCode.Default) después de cargar el archivo de plantilla. Además, guardamos el valor especificado por el usuario (mediante este método) en el archivo también al guardar un archivo XLS. ii). Para otros formatos de archivo, como XLSX, XLSB... etc., no hay un campo definido para la configuración regional en la especificación del formato de archivo. Por lo tanto, utilizamos la configuración regional del entorno de la aplicación para el libro de trabajo. Y el valor especificado por el usuario (mediante este método) no puede conservarse en los archivos generados con esos formatos. 2. Para el efecto de visualización en MS Excel: la configuración regional aplicada aquí solo puede tener efecto en tiempo de ejecución con el componente Aspose.Cells y no al visualizar el archivo generado con MS Excel. Incluso para el archivo XLS generado en el que se han guardado los datos de configuración regional especificados, al visualizar/editarlo con MS Excel, la región utilizada por MS Excel para formatear siempre es la configuración regional predeterminada del entorno donde se ejecuta MS Excel, no la que está guardada en el archivo. Es un comportamiento de MS Excel y no puede ser modificado por código.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Verdadero si la información personal puede eliminarse del workbook especificado.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Establece el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Establece cómo la aplicación muestra las formas en este libro de trabajo.

Ver [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Establece un valor que indica si el libro de trabajo está compartido.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Establece un valor que indica si se muestran las pestañas del libro de trabajo.

**Remarks**

El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Establece el número de dígitos significativos. El valor predeterminado es [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Esta propiedad será eliminada 12 meses después, a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Establece el tipo de dígitos significativos para la salida de valores numéricos en este libro de trabajo. El valor predeterminado es [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Ver [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Establece el proveedor de flujo para recursos externos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ResourceProvider. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Indica si se actualiza el borde de las celdas adyacentes.

**Remarks**

El valor predeterminado es false. Por ejemplo: el borde inferior de la celda A1 se actualiza, el borde superior de la celda A2 también debe cambiarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Establece cómo se actualizan los enlaces externos cuando se abre el libro de trabajo.

Ver [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical.

**Remarks**

El valor predeterminado es true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


La altura de la ventana, en unidades de punto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


La altura de la ventana, en unidades de centímetro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


La altura de la ventana, en unidad de pulgada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidad de punto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de punto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de centímetro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidad de pulgada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


El ancho de la ventana, en unidad de punto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


El ancho de la ventana, en unidad de centímetro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


El ancho de la ventana, en unidad de pulgada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indica si debe ser compatible con WPS.

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

