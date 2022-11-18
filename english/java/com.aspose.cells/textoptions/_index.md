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
## Constructors

| Constructor | Description |
| --- | --- |
| [TextOptions()](#TextOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Checks if two fonts are equals. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Gets and sets the color with a 32-bit ARGB value. |
| [getCapsType()](#getCapsType--) | Gets and sets the text caps type. |
| [getCharset()](#getCharset--) | Represent the character set. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets or sets the [Color](../../com.aspose.cells/color) of the font. |
| [getDoubleSize()](#getDoubleSize--) | Gets and sets the double size of the font. |
| [getFarEastName()](#getFarEastName--) | Gets and sets the FarEast name. |
| [getFill()](#getFill--) | Represents the fill format of the text. |
| [getKerning()](#getKerning--) | Specifies the minimum font size at which character kerning will occur for this text run. |
| [getLanguageCode()](#getLanguageCode--) | Gets and sets the user interface language. |
| [getLatinName()](#getLatinName--) | Gets and sets the latin name. |
| [getName()](#getName--) | Gets and sets the name of the shape. |
| [getOutline()](#getOutline--) | Represents the outline format of the text. |
| [getSchemeType()](#getSchemeType--) | Gets and sets the scheme type of the font. |
| [getScriptOffset()](#getScriptOffset--) | Gets and sets the script offset,in unit of percentage |
| [getShadow()](#getShadow--) | Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape. |
| [getSize()](#getSize--) | Gets or sets the size of the font. |
| [getSpacing()](#getSpacing--) | Specifies the spacing between characters within a text run. |
| [getStrikeType()](#getStrikeType--) | Gets the strike type of the text. |
| [getThemeColor()](#getThemeColor--) | Gets and sets the theme color. |
| [getUnderline()](#getUnderline--) | Gets or sets the font underline type. |
| [getUnderlineColor()](#getUnderlineColor--) | Gets or sets the color of underline. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Gets or sets a value indicating whether the font is bold. |
| [isItalic()](#isItalic--) | Gets or sets a value indicating whether the font is italic. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indicates whether the normalization of height that is to be applied to the text run. |
| [isStrikeout()](#isStrikeout--) | Gets or sets a value indicating whether the font is single strikeout. |
| [isSubscript()](#isSubscript--) | Gets or sets a value indicating whether the font is subscript. |
| [isSuperscript()](#isSuperscript--) | Gets or sets a value indicating whether the font is super script. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | For the description of this property, please see \#getArgbColor().getArgbColor() |
| [setBold(boolean value)](#setBold-boolean-) | For the description of this property, please see \#isBold().isBold() |
| [setCapsType(int value)](#setCapsType-int-) | For the description of this property, please see \#getCapsType().getCapsType() |
| [setCharset(int value)](#setCharset-int-) | For the description of this property, please see \#getCharset().getCharset() |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | For the description of this property, please see \#getColor().getColor() |
| [setDoubleSize(double value)](#setDoubleSize-double-) | For the description of this property, please see \#getDoubleSize().getDoubleSize() |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | For the description of this property, please see \#getFarEastName().getFarEastName() |
| [setItalic(boolean value)](#setItalic-boolean-) | For the description of this property, please see \#isItalic().isItalic() |
| [setKerning(double value)](#setKerning-double-) | For the description of this property, please see \#getKerning().getKerning() |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see \#getLanguageCode().getLanguageCode() |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | For the description of this property, please see \#getLatinName().getLatinName() |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see \#getName().getName() |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | For the description of this property, please see \#isNormalizeHeights().isNormalizeHeights() |
| [setSchemeType(int value)](#setSchemeType-int-) | For the description of this property, please see \#getSchemeType().getSchemeType() |
| [setScriptOffset(double value)](#setScriptOffset-double-) | For the description of this property, please see \#getScriptOffset().getScriptOffset() |
| [setSize(int value)](#setSize-int-) | For the description of this property, please see \#getSize().getSize() |
| [setSpacing(double value)](#setSpacing-double-) | For the description of this property, please see \#getSpacing().getSpacing() |
| [setStrikeType(int value)](#setStrikeType-int-) | For the description of this property, please see \#getStrikeType().getStrikeType() |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | For the description of this property, please see \#isStrikeout().isStrikeout() |
| [setSubscript(boolean value)](#setSubscript-boolean-) | For the description of this property, please see \#isSubscript().isSubscript() |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | For the description of this property, please see \#isSuperscript().isSuperscript() |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | For the description of this property, please see \#getThemeColor().getThemeColor() |
| [setUnderline(int value)](#setUnderline-int-) | For the description of this property, please see \#getUnderline().getUnderline() |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | For the description of this property, please see \#getUnderlineColor().getUnderlineColor() |
| [toString()](#toString--) | Returns a string represents the current Cell object. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


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


Gets and sets the color with a 32-bit ARGB value.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Gets and sets the text caps type.

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


Gets or sets the [Color](../../com.aspose.cells/color) of the font.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Gets and sets the double size of the font.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Gets and sets the FarEast name.

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


Gets and sets the user interface language.

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Gets and sets the latin name.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Gets and sets the name of the shape.

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


Gets and sets the scheme type of the font.

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Gets and sets the script offset,in unit of percentage

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


Gets or sets the size of the font.

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


Gets and sets the theme color. If the font color is not a theme color, NULL will be returned.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Gets or sets the font underline type.

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Gets or sets the color of underline.

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


Gets or sets a value indicating whether the font is bold.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Gets or sets a value indicating whether the font is italic.

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


Gets or sets a value indicating whether the font is single strikeout.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Gets or sets a value indicating whether the font is subscript.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Gets or sets a value indicating whether the font is super script.

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


For the description of this property, please see \#getArgbColor().getArgbColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


For the description of this property, please see \#isBold().isBold()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


For the description of this property, please see \#getCapsType().getCapsType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


For the description of this property, please see \#getCharset().getCharset()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


For the description of this property, please see \#getColor().getColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


For the description of this property, please see \#getDoubleSize().getDoubleSize()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


For the description of this property, please see \#getFarEastName().getFarEastName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


For the description of this property, please see \#isItalic().isItalic()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


For the description of this property, please see \#getKerning().getKerning()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


For the description of this property, please see \#getLanguageCode().getLanguageCode()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


For the description of this property, please see \#getLatinName().getLatinName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see \#getName().getName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


For the description of this property, please see \#isNormalizeHeights().isNormalizeHeights()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


For the description of this property, please see \#getSchemeType().getSchemeType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


For the description of this property, please see \#getScriptOffset().getScriptOffset()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


For the description of this property, please see \#getSize().getSize()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


For the description of this property, please see \#getSpacing().getSpacing()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


For the description of this property, please see \#getStrikeType().getStrikeType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


For the description of this property, please see \#isStrikeout().isStrikeout()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


For the description of this property, please see \#isSubscript().isSubscript()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


For the description of this property, please see \#isSuperscript().isSuperscript()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


For the description of this property, please see \#getThemeColor().getThemeColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


For the description of this property, please see \#getUnderline().getUnderline()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


For the description of this property, please see \#getUnderlineColor().getUnderlineColor()

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

