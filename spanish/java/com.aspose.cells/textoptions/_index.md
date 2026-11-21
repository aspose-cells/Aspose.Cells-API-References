---
title: "TextOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de texto."
type: docs
url: /es/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Representa las opciones de texto.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Comprueba si dos fuentes son iguales. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Obtiene el color con un valor ARGB de 32 bits. |
| [getCapsType()](#getCapsType--) | Obtiene el tipo de mayúsculas para los textos de la forma. |
| [getCharset()](#getCharset--) | Representa el conjunto de caracteres. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtiene el [Color](../../com.aspose.cells/color) de la fuente. |
| [getDoubleSize()](#getDoubleSize--) | Obtiene el tamaño doble de la fuente. |
| [getFarEastName()](#getFarEastName--) | Obtiene el nombre FarEast. |
| [getFill()](#getFill--) | Representa el formato de relleno del texto. |
| [getKerning()](#getKerning--) | Especifica el tamaño mínimo de fuente en el que se producirá el kerning de caracteres para esta ejecución de texto. |
| [getLanguageCode()](#getLanguageCode--) | Obtiene el idioma de la interfaz de usuario. |
| [getLatinName()](#getLatinName--) | Obtiene el nombre latino. |
| [getName()](#getName--) | Obtiene el nombre de la forma. |
| [getOutline()](#getOutline--) | Representa el formato de contorno del texto. |
| [getSchemeType()](#getSchemeType--) | Obtiene el tipo de esquema de la fuente. |
| [getScriptOffset()](#getScriptOffset--) | Obtiene el desplazamiento del script, en unidades de porcentaje |
| [getShadow()](#getShadow--) | Representa un objeto [ShadowEffect](../../com.aspose.cells/shadoweffect) que especifica el efecto de sombra para el elemento de gráfico o forma. |
| [getSize()](#getSize--) | Obtiene el tamaño de la fuente. |
| [getSpacing()](#getSpacing--) | Especifica el espaciado entre caracteres dentro de una ejecución de texto. |
| [getStrikeType()](#getStrikeType--) | Obtiene el tipo de tachado del texto. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getUnderline()](#getUnderline--) | Obtiene el tipo de subrayado de la fuente. |
| [getUnderlineColor()](#getUnderlineColor--) | Obtiene el color del subrayado. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Obtiene un valor que indica si la fuente está en negrita. |
| [isItalic()](#isItalic--) | Obtiene un valor que indica si la fuente está en cursiva. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indica si la normalización de altura debe aplicarse a la ejecución de texto. |
| [isStrikeout()](#isStrikeout--) | Obtiene un valor que indica si la fuente tiene tachado simple. |
| [isSubscript()](#isSubscript--) | Obtiene un valor que indica si la fuente está en subíndice. |
| [isSuperscript()](#isSuperscript--) | Obtiene un valor que indica si la fuente está en superíndice. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Establece el color con un valor ARGB de 32 bits. |
| [setBold(boolean value)](#setBold-boolean-) | Establece un valor que indica si la fuente está en negrita. |
| [setCapsType(int value)](#setCapsType-int-) | Establece el tipo de mayúsculas para los textos de la forma. |
| [setCharset(int value)](#setCharset-int-) | Representa el conjunto de caracteres. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Establece el [Color](../../com.aspose.cells/color) de la fuente. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Establece el doble tamaño de la fuente. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Establece el nombre FarEast. |
| [setItalic(boolean value)](#setItalic-boolean-) | Establece un valor que indica si la fuente está en cursiva. |
| [setKerning(double value)](#setKerning-double-) | Especifica el tamaño mínimo de fuente en el que se producirá el kerning de caracteres para esta ejecución de texto. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Establece el idioma de la interfaz de usuario. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Establece el nombre latino. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la forma. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Establece el nombre y el esquema de la fuente. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indica si la normalización de altura debe aplicarse a la ejecución de texto. |
| [setSchemeType(int value)](#setSchemeType-int-) | Establece el tipo de esquema de la fuente. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Establece el desplazamiento del script, en unidades de porcentaje. |
| [setSize(int value)](#setSize-int-) | Establece el tamaño de la fuente. |
| [setSpacing(double value)](#setSpacing-double-) | Especifica el espaciado entre caracteres dentro de una ejecución de texto. |
| [setStrikeType(int value)](#setStrikeType-int-) | Obtiene el tipo de tachado del texto. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Establece un valor que indica si la fuente tiene un tachado simple. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Establece un valor que indica si la fuente está en subíndice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Establece un valor que indica si la fuente está en superíndice. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Establece el color del tema. |
| [setUnderline(int value)](#setUnderline-int-) | Establece el tipo de subrayado de la fuente. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Establece el color del subrayado. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Cell actual. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Comprueba si dos fuentes son iguales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Objeto de fuente comparado. |

**Returns:**
booleano - Verdadero si es igual al objeto de fuente comparado.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Obtiene el color con un valor ARGB de 32 bits.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Obtiene el tipo de mayúsculas para los textos de la forma.

Ver [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Representa el conjunto de caracteres.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Obtiene el [Color](../../com.aspose.cells/color) de la fuente.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Obtiene el tamaño doble de la fuente.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Obtiene el nombre FarEast.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Representa el formato de relleno del texto.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Especifica el tamaño mínimo de fuente en el que se producirá el kerning de caracteres para esta ejecución de texto.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Obtiene el idioma de la interfaz de usuario.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Obtiene el nombre latino.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la forma.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Representa el formato de contorno del texto.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Obtiene el tipo de esquema de la fuente.

Ver [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Obtiene el desplazamiento del script, en unidades de porcentaje

**Remarks**

Solo para formas y gráficos.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Representa un objeto [ShadowEffect](../../com.aspose.cells/shadoweffect) que especifica el efecto de sombra para el elemento de gráfico o forma.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Obtiene el tamaño de la fuente.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Especifica el espaciado entre caracteres dentro de una ejecución de texto.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Obtiene el tipo de tachado del texto.

Ver [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtiene el color del tema.

**Remarks**

Si el color de la fuente no es un color de tema, se devolverá NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Obtiene el tipo de subrayado de la fuente.

Ver [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Obtiene el color del subrayado.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Obtiene un valor que indica si la fuente está en negrita.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtiene un valor que indica si la fuente está en cursiva.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indica si la normalización de altura debe aplicarse a la ejecución de texto.

**Remarks**

Solo para las fuentes de Formas o Gráficos.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Obtiene un valor que indica si la fuente tiene tachado simple.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Obtiene un valor que indica si la fuente está en subíndice.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Obtiene un valor que indica si la fuente está en superíndice.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Establece el color con un valor ARGB de 32 bits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Establece un valor que indica si la fuente está en negrita.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Establece el tipo de mayúsculas para los textos de la forma.

Ver [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Representa el conjunto de caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Establece el [Color](../../com.aspose.cells/color) de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Establece el doble tamaño de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Establece el nombre FarEast.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Establece un valor que indica si la fuente está en cursiva.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Especifica el tamaño mínimo de fuente en el que se producirá el kerning de caracteres para esta ejecución de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Establece el idioma de la interfaz de usuario.

Ver [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Establece el nombre latino.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Establece el nombre y el esquema de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indica si la normalización de altura debe aplicarse a la ejecución de texto.

**Remarks**

Solo para las fuentes de Formas o Gráficos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Establece el tipo de esquema de la fuente.

Ver [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Establece el desplazamiento del script, en unidades de porcentaje.

**Remarks**

Solo para formas y gráficos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Establece el tamaño de la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Especifica el espaciado entre caracteres dentro de una ejecución de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Obtiene el tipo de tachado del texto.

Ver [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Establece un valor que indica si la fuente tiene un tachado simple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Establece un valor que indica si la fuente está en subíndice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Establece un valor que indica si la fuente está en superíndice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Establece el color del tema.

**Remarks**

Si el color de la fuente no es un color de tema, se devolverá NULL.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Establece el tipo de subrayado de la fuente.

Ver [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Establece el color del subrayado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Cell actual.

**Returns:**
java.lang.String -
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

