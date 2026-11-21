---
title: "Style"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el estilo de visualización de documentos de Excel, como fuente, color, alineación, borde, etc."
type: docs
url: /es/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Representa el estilo de visualización de un documento de Excel, como fuente, color, alineación, borde, etc. El objeto Style contiene todos los atributos de estilo (fuente, formato numérico, alineación, etc.) como propiedades.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Style()](#Style--) | Inicializa una nueva instancia de la clase [Style](../../com.aspose.cells/style). |
## Métodos

| Método | Descripción |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Copia datos de otro objeto Style. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si dos instancias de Style son iguales. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Obtiene el color de fondo con un valor ARGB de 32 bits. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtiene el color de fondo de un estilo. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Obtiene el color de tema de fondo. |
| [getBorders()](#getBorders--) | Obtiene la [BorderCollection](../../com.aspose.cells/bordercollection) del estilo. |
| [getBottomBorder()](#getBottomBorder--) | Obtiene el borde inferior. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Obtiene la cadena de patrón dependiente de la cultura para el formato numérico. |
| [getCustom()](#getCustom--) | Representa la cadena de formato numérico personalizado de este objeto Style. |
| [getFont()](#getFont--) | Obtiene un objeto [getFont()](../../com.aspose.cells/style\#getFont--). |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Obtiene el color de primer plano con un valor ARGB de 32 bits. |
| [getForegroundColor()](#getForegroundColor--) | Obtiene el color de primer plano de un estilo. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Obtiene el color de tema de primer plano. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Obtiene el tipo de alineación horizontal del texto en una celda. |
| [getIndentLevel()](#getIndentLevel--) | Representa el nivel de sangría para la celda o el rango. |
| [getInvariantCustom()](#getInvariantCustom--) | Obtiene la cadena de patrón independiente de la cultura para el formato numérico. |
| [getLeftBorder()](#getLeftBorder--) | Obtiene el borde izquierdo. |
| [getName()](#getName--) | Obtiene el nombre del estilo. |
| [getNumber()](#getNumber--) | Obtiene el formato de visualización de números y fechas. |
| [getParentStyle()](#getParentStyle--) | Obtiene el estilo padre de este estilo. |
| [getPattern()](#getPattern--) | Obtiene el tipo de patrón de fondo de la celda. |
| [getQuotePrefix()](#getQuotePrefix--) | Indica si el valor de la celda comienza con una comilla simple. |
| [getRightBorder()](#getRightBorder--) | Obtiene el borde derecho. |
| [getRotationAngle()](#getRotationAngle--) | Representa el ángulo de rotación del texto. |
| [getShrinkToFit()](#getShrinkToFit--) | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible. |
| [getTextDirection()](#getTextDirection--) | Representa el orden de lectura del texto. |
| [getTopBorder()](#getTopBorder--) | Obtiene el borde superior. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Obtiene la configuración de degradado de dos colores. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Obtiene la configuración de degradado de dos colores. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Obtiene el tipo de alineación vertical del texto en una celda. |
| [hasBorders()](#hasBorders--) | Comprueba si se han establecido bordes para el estilo. |
| [hashCode()](#hashCode--) | Sirve como función hash para un objeto Style. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Indica si se debe aplicar el formato de alineación. |
| [isBorderApplied()](#isBorderApplied--) | Indica si se debe aplicar el formato de borde. |
| [isCheckBox()](#isCheckBox--) | Indica si es un estilo de casilla de verificación |
| [isDateTime()](#isDateTime--) | Indica si el formato numérico es un formato de fecha. |
| [isFillApplied()](#isFillApplied--) | Indica si se debe aplicar el formato de relleno. |
| [isFontApplied()](#isFontApplied--) | Indica si se debe aplicar el formato de fuente. |
| [isFormulaHidden()](#isFormulaHidden--) | Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida. |
| [isGradient()](#isGradient--) | Indica si el sombreado de la celda es un patrón degradado. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto. |
| [isLocked()](#isLocked--) | Obtiene un valor que indica si una celda puede modificarse o no. |
| [isModified(int modifyFlag)](#isModified-int-) | Comprueba si las propiedades especificadas del estilo han sido modificadas. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Indica si se debe aplicar el formato numérico. |
| [isPercent()](#isPercent--) | Indica si el formato numérico es un formato de porcentaje. |
| [isProtectionApplied()](#isProtectionApplied--) | Indica si se debe aplicar el formato de protección. |
| [isTextWrapped()](#isTextWrapped--) | Obtiene un valor que indica si el texto dentro de una celda está ajustado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Indica si se debe aplicar el formato de alineación. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Establece el color de fondo con un valor ARGB de 32 bits. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Establece el color de fondo de un estilo. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Establece el color de tema de fondo. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Establece los bordes del estilo. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Establece los bordes del estilo. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Indica si se debe aplicar el formato de borde. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Indica si es un estilo de casilla de verificación |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Establece la cadena de patrón dependiente de la cultura para el formato numérico. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Representa la cadena de formato numérico personalizado de este objeto Style. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Establece la cadena de formato numérico personalizado de una celda. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Indica si se debe aplicar el formato de relleno. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Indica si se debe aplicar el formato de fuente. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Establece el color de primer plano con un valor ARGB de 32 bits. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Establece el color de primer plano de un estilo. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Establece el color de tema de primer plano. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida. |
| [setGradient(boolean value)](#setGradient-boolean-) | Indica si el sombreado de la celda es un patrón degradado. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Establece el tipo de alineación horizontal del texto en una celda. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Representa el nivel de sangría para la celda o el rango. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto. |
| [setLocked(boolean value)](#setLocked-boolean-) | Establece un valor que indica si una celda puede modificarse o no. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre del estilo. |
| [setNumber(int value)](#setNumber-int-) | Establece el formato de visualización de números y fechas. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Indica si se debe aplicar el formato numérico. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Establece los bordes de contorno |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Establece los bordes de contorno |
| [setPattern(int value)](#setPattern-int-) | Establece el tipo de patrón de fondo de la celda. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Establece el color de fondo. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Indica si se debe aplicar el formato de protección. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indica si el valor de la celda comienza con una comilla simple. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representa el ángulo de rotación del texto. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representa el orden de lectura del texto. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Establece un valor que indica si el texto dentro de una celda está ajustado. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Establece el relleno especificado a un degradado de dos colores. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Establece el tipo de alineación vertical del texto en una celda. |
| [toJson()](#toJson--) | Convierte [Style](../../com.aspose.cells/style) a datos de estructura JSON. |
| [toString()](#toString--) |  |
| [update()](#update--) | Aplica el estilo nombrado a los estilos de las celdas que usan este estilo nombrado. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Inicializa una nueva instancia de la clase [Style](../../com.aspose.cells/style).

**Remarks**

NOTA: Este constructor está ahora obsoleto. En su lugar, utilice el método CellsFactory.CreateStyle(). Esta propiedad será eliminada 6 meses después desde octubre de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Copia datos de otro objeto Style.

**Remarks**

Este método no copia el nombre del estilo. Si desea copiar el nombre, llame al siguiente código después de copiar el estilo: destStyle.Name = style.Name.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Objeto Style de origen |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si dos instancias de Style son iguales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto Style para comparar con el objeto Style actual. |

**Returns:**
boolean - true si el Object especificado es igual al Object actual; de lo contrario, false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Obtiene el color de fondo con un valor ARGB de 32 bits.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Obtiene el color de fondo de un estilo.

**Remarks**

Si desea establecer el color de una celda, utilice la propiedad Style.ForegroundColor. Sólo si el patrón de estilo de la celda es distinto de ninguno o sólido, esta propiedad tendrá efecto.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Obtiene el color de tema de fondo.

**Remarks**

Si el color de fondo no es un color de tema, se devolverá NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Obtiene la [BorderCollection](../../com.aspose.cells/bordercollection) del estilo.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Obtiene el borde inferior.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


Obtiene la cadena de patrón dependiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado.

**Remarks**

Para los formatos numéricos incorporados, tanto el contenido del patrón (por ejemplo, un formato de fecha incorporado es "m/d/y" para algunas configuraciones regionales, pero para otras se convierte en "d/m/y") como el especificador de formato (por ejemplo, algunas configuraciones regionales usan un carácter distinto de 'y' para representar la parte del año en el formato de fecha) dependen de la cultura; para un formato personalizado especificado por el usuario, sólo los especificadores de formato se cambian según la cultura, las demás partes del patrón de formato no se modifican.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Representa la cadena de formato numérico personalizado de este objeto style. Si el formato numérico personalizado no está establecido (por ejemplo, el formato numérico es incorporado), se devolverá "".

**Remarks**

La cadena personalizada devuelta es independiente de la cultura.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Obtiene un objeto [getFont()](../../com.aspose.cells/style\#getFont--).

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Obtiene el color de primer plano con un valor ARGB de 32 bits.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Obtiene el color de primer plano de un estilo.

**Remarks**

Significa que no hay configuración de color si se devuelve Color.Empty.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Obtiene el color de tema de primer plano.

**Remarks**

Si el color de primer plano no es un color de tema, se devolverá NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Obtiene el tipo de alineación horizontal del texto en una celda.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Representa el nivel de sangría para la celda o rango. Sólo puede ser un entero de 0 a 250.

**Remarks**

Si el tipo de alineación horizontal del texto se establece a un valor distinto de izquierda o derecha, el nivel de sangría se restablecerá a cero.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Obtiene la cadena de patrón independiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado.

**Remarks**

Para los formatos numéricos incorporados, el contenido del patrón devuelto sigue siendo dependiente de la cultura, por ejemplo, para algunas configuraciones regionales devuelve "m/d/y" y para otras devuelve "d/m/y". La diferencia con [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) es (eso también es lo que significa independiente de la cultura): los especificadores de formato y separadores se mantienen como estándar, por ejemplo '/' siempre se usará como separador de fecha y hora y "y" siempre se usará como la parte de "año" sin importar qué otro carácter especial se use para la configuración regional específica.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Obtiene el borde izquierdo.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del estilo.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Obtiene el formato de visualización de números y fechas. Los patrones de formato son diferentes para distintas regiones.

**Remarks**

Por ejemplo, los patrones de formato representados por números para la región en\_US:

| Value | Tipo | Cadena de formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Obtiene el estilo padre de este estilo.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Obtiene el tipo de patrón de fondo de la celda.

Ver [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indica si el valor de la celda comienza con una comilla simple.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Obtiene el borde derecho.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representa el ángulo de rotación del texto.

**Remarks**

0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.

Puede establecer 255 o un valor en el rango de -90 a 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Obtiene el borde superior.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Obtiene la configuración de degradado de dos colores.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Style.GetTwoColorGradientSetting(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.Object[] - Devuelve todas las configuraciones sobre el degradado de dos colores [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Obtiene la configuración de degradado de dos colores.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Obtiene el tipo de alineación vertical del texto en una celda.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Comprueba si se han establecido bordes para el estilo.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Sirve como función hash para un objeto Style.

**Remarks**

Este método es solo para uso interno.

**Returns:**
int - Un código hash para el objeto actual.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Indica si se debe aplicar el formato de alineación.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Indica si se debe aplicar el formato de borde.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Indica si es un estilo de casilla de verificación

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Indica si el formato numérico es un formato de fecha.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Indica si se debe aplicar el formato de relleno.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Indica si se debe aplicar el formato de fuente.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Indica si el sombreado de la celda es un patrón degradado.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto.

**Remarks**

Esto es típico para alineaciones de Asia Oriental pero no es típico en otros contextos. Solo funciona cuando la alineación horizontal está distribuida.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Obtiene un valor que indica si una celda puede modificarse o no.

**Remarks**

Bloquear celdas no tiene efecto a menos que la hoja de cálculo esté protegida.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Comprueba si las propiedades especificadas del estilo han sido modificadas. Se utiliza para el estilo de ConditionalFormattings para verificar si las propiedades especificadas de este estilo deben usarse al aplicar ConditionalFormattings en una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Banderas de estilo modificado. |

**Returns:**
boolean - verdadero si las propiedades especificadas han sido modificadas
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Indica si se debe aplicar el formato numérico.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Indica si el formato numérico es un formato de porcentaje.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Indica si se debe aplicar el formato de protección.

**Remarks**

Solo para estilo con nombre.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtiene un valor que indica si el texto dentro de una celda está ajustado.

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




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


Indica si se debe aplicar el formato de alineación.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Establece el color de fondo con un valor ARGB de 32 bits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Establece el color de fondo de un estilo.

**Remarks**

Si desea establecer el color de una celda, utilice la propiedad Style.ForegroundColor. Sólo si el patrón de estilo de la celda es distinto de ninguno o sólido, esta propiedad tendrá efecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Establece el color de tema de fondo.

**Remarks**

Si el color de fondo no es un color de tema, se devolverá NULL.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Establece los bordes del estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). El/los borde(s) a establecer, puede ser una combinación de [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). El estilo del borde. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | El color del borde. |

**Returns:**
boolean - Si la configuración actual del borde ha sido cambiada.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Establece los bordes del estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). El/los borde(s) a establecer, puede ser una combinación de [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). El estilo del borde. |
| borderColor | [Color](../../com.aspose.cells/color) | El color del borde. |

**Returns:**
boolean - Si la configuración actual del borde ha sido cambiada.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Indica si se debe aplicar el formato de borde.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Indica si es un estilo de casilla de verificación

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Establece la cadena de patrón dependiente de la cultura para el formato numérico. Si no se ha establecido ningún formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado.

**Remarks**

Para los formatos numéricos incorporados, tanto el contenido del patrón (por ejemplo, un formato de fecha incorporado es "m/d/y" para algunas configuraciones regionales, pero para otras se convierte en "d/m/y") como el especificador de formato (por ejemplo, algunas configuraciones regionales usan un carácter distinto de 'y' para representar la parte del año en el formato de fecha) dependen de la cultura; para un formato personalizado especificado por el usuario, sólo los especificadores de formato se cambian según la cultura, las demás partes del patrón de formato no se modifican.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Representa la cadena de formato numérico personalizado de este objeto style. Si el formato numérico personalizado no está establecido (por ejemplo, el formato numérico es incorporado), se devolverá "".

**Remarks**

La cadena personalizada devuelta es independiente de la cultura.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Establece la cadena de formato numérico personalizado de una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| personalizado | java.lang.String | Cadena de formato numérico personalizada, debe ser un patrón InvariantCulture. |
| builtinPreference | boolean | Si la cadena de formato numérico personalizada proporcionada coincide con uno de los formatos numéricos incorporados correspondientes a la configuración regional actual, establecer el formato numérico como incorporado en lugar de personalizado. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Indica si se debe aplicar el formato de relleno.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Indica si se debe aplicar el formato de fuente.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Establece el color de primer plano con un valor ARGB de 32 bits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Establece el color de primer plano de un estilo.

**Remarks**

Significa que no hay configuración de color si se devuelve Color.Empty.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Establece el color de tema de primer plano.

**Remarks**

Si el color de primer plano no es un color de tema, se devolverá NULL.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Indica si el sombreado de la celda es un patrón degradado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Establece el tipo de alineación horizontal del texto en una celda.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Representa el nivel de sangría para la celda o rango. Sólo puede ser un entero de 0 a 250.

**Remarks**

Si el tipo de alineación horizontal del texto se establece a un valor distinto de izquierda o derecha, el nivel de sangría se restablecerá a cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto.

**Remarks**

Esto es típico para alineaciones de Asia Oriental pero no es típico en otros contextos. Solo funciona cuando la alineación horizontal está distribuida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Establece un valor que indica si una celda puede modificarse o no.

**Remarks**

Bloquear celdas no tiene efecto a menos que la hoja de cálculo esté protegida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre del estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Establece el formato de visualización de números y fechas. Los patrones de formato son diferentes para distintas regiones.

**Remarks**

Por ejemplo, los patrones de formato representados por números para la región en\_US:

| Value | Tipo | Cadena de formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Indica si se debe aplicar el formato numérico.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Establece los bordes de contorno

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). El tipo de bordes. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | El color de los bordes |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Establece los bordes de contorno

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). El tipo de bordes. |
| borderColor | [Color](../../com.aspose.cells/color) | El color de los bordes |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Establece el tipo de patrón de fondo de la celda.

Ver [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Establece el color de fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). El patrón. |
| color1 | [Color](../../com.aspose.cells/color) | El color de primer plano. |
| color2 | [Color](../../com.aspose.cells/color) | El color de fondo. Sólo funciona cuando el patrón no es BackgroundType.None y BackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Indica si se debe aplicar el formato de protección.

**Remarks**

Solo para estilo con nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indica si el valor de la celda comienza con una comilla simple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representa el ángulo de rotación del texto.

**Remarks**

0: No rotado.

255: De arriba a abajo.

\-90: Hacia abajo.

90: Hacia arriba.

Puede establecer 255 o un valor en el rango de -90 a 90.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Representa el orden de lectura del texto.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Establece un valor que indica si el texto dentro de una celda está ajustado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Establece el relleno especificado a un degradado de dos colores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un color de degradado. |
| color2 | [Color](../../com.aspose.cells/color) | Dos colores de degradado. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Establece el tipo de alineación vertical del texto en una celda.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Convierte [Style](../../com.aspose.cells/style) a datos de estructura JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


Aplica el estilo nombrado a los estilos de las celdas que usan este estilo nombrado. Funciona como hacer clic en el botón "ok" después de terminar de modificar el estilo. Sólo se aplica al estilo nombrado.

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

