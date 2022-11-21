---
title: TextOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the text options.
type: docs
weight: 577
url: /java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Represents the text options.
## Methods

| Method | Description |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Checks if two fonts are equals. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | the color with a 32-bit ARGB value. |
| [getCapsType()](#getCapsType--) | the text caps type. |
| [getCharset()](#getCharset--) | Represent the character set. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | the [Color](../../com.aspose.cells/color) of the font. |
| [getDoubleSize()](#getDoubleSize--) | the double size of the font. |
| [getFarEastName()](#getFarEastName--) | the FarEast name. |
| [getFill()](#getFill--) | Represents the fill format of the text. |
| [getKerning()](#getKerning--) | Specifies the minimum font size at which character kerning will occur for this text run. |
| [getLanguageCode()](#getLanguageCode--) | the user interface language. |
| [getLatinName()](#getLatinName--) | the latin name. |
| [getName()](#getName--) | the name of the shape. |
| [getOutline()](#getOutline--) | Represents the outline format of the text. |
| [getSchemeType()](#getSchemeType--) | the scheme type of the font. |
| [getScriptOffset()](#getScriptOffset--) | the script offset,in unit of percentage |
| [getShadow()](#getShadow--) | Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape. |
| [getSize()](#getSize--) | the size of the font. |
| [getSpacing()](#getSpacing--) | Specifies the spacing between characters within a text run. |
| [getStrikeType()](#getStrikeType--) | Gets the strike type of the text. |
| [getThemeColor()](#getThemeColor--) | the theme color. |
| [getUnderline()](#getUnderline--) | the font underline type. |
| [getUnderlineColor()](#getUnderlineColor--) | the color of underline. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | a value indicating whether the font is bold. |
| [isItalic()](#isItalic--) | a value indicating whether the font is italic. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indicates whether the normalization of height that is to be applied to the text run. |
| [isStrikeout()](#isStrikeout--) | a value indicating whether the font is single strikeout. |
| [isSubscript()](#isSubscript--) | a value indicating whether the font is subscript. |
| [isSuperscript()](#isSuperscript--) | a value indicating whether the font is super script. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | For the description of this property, please see [getArgbColor()](../../com.aspose.cells/font\#getArgbColor--) |
| [setBold(boolean value)](#setBold-boolean-) | For the description of this property, please see [isBold()](../../com.aspose.cells/font\#isBold--) |
| [setCapsType(int value)](#setCapsType-int-) | For the description of this property, please see [getCapsType()](../../com.aspose.cells/font\#getCapsType--) |
| [setCharset(int value)](#setCharset-int-) | For the description of this property, please see [getCharset()](../../com.aspose.cells/font\#getCharset--) |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | For the description of this property, please see [getColor()](../../com.aspose.cells/font\#getColor--) |
| [setDoubleSize(double value)](#setDoubleSize-double-) | For the description of this property, please see [getDoubleSize()](../../com.aspose.cells/font\#getDoubleSize--) |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | For the description of this property, please see [getFarEastName()](../../com.aspose.cells/textoptions\#getFarEastName--) |
| [setItalic(boolean value)](#setItalic-boolean-) | For the description of this property, please see [isItalic()](../../com.aspose.cells/font\#isItalic--) |
| [setKerning(double value)](#setKerning-double-) | For the description of this property, please see [getKerning()](../../com.aspose.cells/textoptions\#getKerning--) |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/textoptions\#getLanguageCode--) |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | For the description of this property, please see [getLatinName()](../../com.aspose.cells/textoptions\#getLatinName--) |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.cells/textoptions\#getName--) |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | For the description of this property, please see [isNormalizeHeights()](../../com.aspose.cells/font\#isNormalizeHeights--) |
| [setSchemeType(int value)](#setSchemeType-int-) | For the description of this property, please see [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) |
| [setScriptOffset(double value)](#setScriptOffset-double-) | For the description of this property, please see [getScriptOffset()](../../com.aspose.cells/font\#getScriptOffset--) |
| [setSize(int value)](#setSize-int-) | For the description of this property, please see [getSize()](../../com.aspose.cells/font\#getSize--) |
| [setSpacing(double value)](#setSpacing-double-) | For the description of this property, please see [getSpacing()](../../com.aspose.cells/textoptions\#getSpacing--) |
| [setStrikeType(int value)](#setStrikeType-int-) | For the description of this property, please see [getStrikeType()](../../com.aspose.cells/font\#getStrikeType--) |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | For the description of this property, please see [isStrikeout()](../../com.aspose.cells/font\#isStrikeout--) |
| [setSubscript(boolean value)](#setSubscript-boolean-) | For the description of this property, please see [isSubscript()](../../com.aspose.cells/font\#isSubscript--) |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | For the description of this property, please see [isSuperscript()](../../com.aspose.cells/font\#isSuperscript--) |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | For the description of this property, please see [getThemeColor()](../../com.aspose.cells/font\#getThemeColor--) |
| [setUnderline(int value)](#setUnderline-int-) | For the description of this property, please see [getUnderline()](../../com.aspose.cells/font\#getUnderline--) |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | For the description of this property, please see [getUnderlineColor()](../../com.aspose.cells/textoptions\#getUnderlineColor--) |
| [toString()](#toString--) | Returns a string represents the current Cell object. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Checks if two fonts are equals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Compared font object. |

**Returns:**
boolean - True if equal to the compared font object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


the color with a 32-bit ARGB value.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


the text caps type.

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Represent the character set.

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


the [Color](../../com.aspose.cells/color) of the font.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


the double size of the font.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


the FarEast name.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Represents the fill format of the text.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Specifies the minimum font size at which character kerning will occur for this text run.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


the user interface language.

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


the latin name.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


the name of the shape.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Represents the outline format of the text.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


the scheme type of the font.

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


the script offset,in unit of percentage

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


the size of the font.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Specifies the spacing between characters within a text run.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Gets the strike type of the text.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


the theme color. If the font color is not a theme color, NULL will be returned.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


the font underline type.

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


the color of underline.

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


a value indicating whether the font is bold.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


a value indicating whether the font is italic.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indicates whether the normalization of height that is to be applied to the text run.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


a value indicating whether the font is single strikeout.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


a value indicating whether the font is subscript.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


a value indicating whether the font is super script.

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


For the description of this property, please see [getArgbColor()](../../com.aspose.cells/font\#getArgbColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


For the description of this property, please see [isBold()](../../com.aspose.cells/font\#isBold--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


For the description of this property, please see [getCapsType()](../../com.aspose.cells/font\#getCapsType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


For the description of this property, please see [getCharset()](../../com.aspose.cells/font\#getCharset--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


For the description of this property, please see [getColor()](../../com.aspose.cells/font\#getColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


For the description of this property, please see [getDoubleSize()](../../com.aspose.cells/font\#getDoubleSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


For the description of this property, please see [getFarEastName()](../../com.aspose.cells/textoptions\#getFarEastName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


For the description of this property, please see [isItalic()](../../com.aspose.cells/font\#isItalic--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


For the description of this property, please see [getKerning()](../../com.aspose.cells/textoptions\#getKerning--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/textoptions\#getLanguageCode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


For the description of this property, please see [getLatinName()](../../com.aspose.cells/textoptions\#getLatinName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.cells/textoptions\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


For the description of this property, please see [isNormalizeHeights()](../../com.aspose.cells/font\#isNormalizeHeights--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


For the description of this property, please see [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


For the description of this property, please see [getScriptOffset()](../../com.aspose.cells/font\#getScriptOffset--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


For the description of this property, please see [getSize()](../../com.aspose.cells/font\#getSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


For the description of this property, please see [getSpacing()](../../com.aspose.cells/textoptions\#getSpacing--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


For the description of this property, please see [getStrikeType()](../../com.aspose.cells/font\#getStrikeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


For the description of this property, please see [isStrikeout()](../../com.aspose.cells/font\#isStrikeout--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


For the description of this property, please see [isSubscript()](../../com.aspose.cells/font\#isSubscript--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


For the description of this property, please see [isSuperscript()](../../com.aspose.cells/font\#isSuperscript--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


For the description of this property, please see [getThemeColor()](../../com.aspose.cells/font\#getThemeColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


For the description of this property, please see [getUnderline()](../../com.aspose.cells/font\#getUnderline--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


For the description of this property, please see [getUnderlineColor()](../../com.aspose.cells/textoptions\#getUnderlineColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Returns a string represents the current Cell object.

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

