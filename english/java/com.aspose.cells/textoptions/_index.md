---
title: TextOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the text options.
type: docs
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
| [getArgbColor()](#getArgbColor--) | Gets the color with a 32-bit ARGB value. |
| [getCapsType()](#getCapsType--) | Gets the text caps type. |
| [getCharset()](#getCharset--) | Represent the character set. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets the [Color](../../com.aspose.cells/color) of the font. |
| [getDoubleSize()](#getDoubleSize--) | Gets the double size of the font. |
| [getFarEastName()](#getFarEastName--) | Gets the FarEast name. |
| [getFill()](#getFill--) | Represents the fill format of the text. |
| [getKerning()](#getKerning--) | Specifies the minimum font size at which character kerning will occur for this text run. |
| [getLanguageCode()](#getLanguageCode--) | Gets the user interface language. |
| [getLatinName()](#getLatinName--) | Gets the latin name. |
| [getName()](#getName--) | Gets the name of the shape. |
| [getOutline()](#getOutline--) | Represents the outline format of the text. |
| [getSchemeType()](#getSchemeType--) | Gets the scheme type of the font. |
| [getScriptOffset()](#getScriptOffset--) | Gets the script offset,in unit of percentage |
| [getShadow()](#getShadow--) | Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape. |
| [getSize()](#getSize--) | Gets the size of the font. |
| [getSpacing()](#getSpacing--) | Specifies the spacing between characters within a text run. |
| [getStrikeType()](#getStrikeType--) | Gets the strike type of the text. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color. |
| [getUnderline()](#getUnderline--) | Gets the font underline type. |
| [getUnderlineColor()](#getUnderlineColor--) | Gets the color of underline. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Gets a value indicating whether the font is bold. |
| [isItalic()](#isItalic--) | Gets a value indicating whether the font is italic. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indicates whether the normalization of height that is to be applied to the text run. |
| [isStrikeout()](#isStrikeout--) | Gets a value indicating whether the font is single strikeout. |
| [isSubscript()](#isSubscript--) | Gets a value indicating whether the font is subscript. |
| [isSuperscript()](#isSuperscript--) | Gets a value indicating whether the font is super script. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Sets the color with a 32-bit ARGB value. |
| [setBold(boolean value)](#setBold-boolean-) | Sets a value indicating whether the font is bold. |
| [setCapsType(int value)](#setCapsType-int-) | Sets the text caps type. |
| [setCharset(int value)](#setCharset-int-) | Represent the character set. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Sets the [Color](../../com.aspose.cells/color) of the font. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Sets the double size of the font. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Sets the FarEast name. |
| [setItalic(boolean value)](#setItalic-boolean-) | Sets a value indicating whether the font is italic. |
| [setKerning(double value)](#setKerning-double-) | Specifies the minimum font size at which character kerning will occur for this text run. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Sets the user interface language. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Sets the latin name. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the shape. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Sets name and scheme of the font. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indicates whether the normalization of height that is to be applied to the text run. |
| [setSchemeType(int value)](#setSchemeType-int-) | Sets the scheme type of the font. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Sets the script offset,in unit of percentage |
| [setSize(int value)](#setSize-int-) | Sets the size of the font. |
| [setSpacing(double value)](#setSpacing-double-) | Specifies the spacing between characters within a text run. |
| [setStrikeType(int value)](#setStrikeType-int-) | Gets the strike type of the text. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Sets a value indicating whether the font is single strikeout. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Sets a value indicating whether the font is subscript. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Sets a value indicating whether the font is super script. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Sets the theme color. |
| [setUnderline(int value)](#setUnderline-int-) | Sets the font underline type. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Sets the color of underline. |
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


Gets the color with a 32-bit ARGB value.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Gets the text caps type.

See [TextCapsType](../../com.aspose.cells/textcapstype).

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


Gets the [Color](../../com.aspose.cells/color) of the font.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Gets the double size of the font.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Gets the FarEast name.

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


Gets the user interface language.

See [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Gets the latin name.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Gets the name of the shape.

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


Gets the scheme type of the font.

See [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Gets the script offset,in unit of percentage

**Remarks**

Only for shapes and charts.

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


Gets the size of the font.

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

See [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Gets the theme color.

**Remarks**

If the font color is not a theme color, NULL will be returned.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Gets the font underline type.

See [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Gets the color of underline.

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


Gets a value indicating whether the font is bold.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Gets a value indicating whether the font is italic.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indicates whether the normalization of height that is to be applied to the text run.

**Remarks**

Only for the fonts of Shapes or Charts.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Gets a value indicating whether the font is single strikeout.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Gets a value indicating whether the font is subscript.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Gets a value indicating whether the font is super script.

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


Sets the color with a 32-bit ARGB value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Sets a value indicating whether the font is bold.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Sets the text caps type.

See [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Represent the character set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Sets the [Color](../../com.aspose.cells/color) of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Sets the double size of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Sets the FarEast name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Sets a value indicating whether the font is italic.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Specifies the minimum font size at which character kerning will occur for this text run.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Sets the user interface language.

See [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Sets the latin name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sets the name of the shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Sets name and scheme of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indicates whether the normalization of height that is to be applied to the text run.

**Remarks**

Only for the fonts of Shapes or Charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Sets the scheme type of the font.

See [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Sets the script offset,in unit of percentage

**Remarks**

Only for shapes and charts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Sets the size of the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Specifies the spacing between characters within a text run.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Gets the strike type of the text.

See [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Sets a value indicating whether the font is single strikeout.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Sets a value indicating whether the font is subscript.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Sets a value indicating whether the font is super script.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Sets the theme color.

**Remarks**

If the font color is not a theme color, NULL will be returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Sets the font underline type.

See [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Sets the color of underline.

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

