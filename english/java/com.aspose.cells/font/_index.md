---
title: Font
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the font object used in a spreadsheet.
type: docs
url: /java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Encapsulates the font object used in a spreadsheet.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
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
| [getName()](#getName--) | Gets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--). |
| [getSchemeType()](#getSchemeType--) | Gets the scheme type of the font. |
| [getScriptOffset()](#getScriptOffset--) | Gets the script offset,in unit of percentage |
| [getSize()](#getSize--) | Gets the size of the font. |
| [getStrikeType()](#getStrikeType--) | Gets the strike type of the text. |
| [getThemeColor()](#getThemeColor--) | Gets the theme color. |
| [getUnderline()](#getUnderline--) | Gets the font underline type. |
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
| [setItalic(boolean value)](#setItalic-boolean-) | Sets a value indicating whether the font is italic. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Sets name and scheme of the font. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indicates whether the normalization of height that is to be applied to the text run. |
| [setSchemeType(int value)](#setSchemeType-int-) | Sets the scheme type of the font. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Sets the script offset,in unit of percentage |
| [setSize(int value)](#setSize-int-) | Sets the size of the font. |
| [setStrikeType(int value)](#setStrikeType-int-) | Gets the strike type of the text. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Sets a value indicating whether the font is single strikeout. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Sets a value indicating whether the font is subscript. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Sets a value indicating whether the font is super script. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Sets the theme color. |
| [setUnderline(int value)](#setUnderline-int-) | Sets the font underline type. |
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

**Remarks**

Only for the fonts of Shapes or Charts. NOTE: This member is now obsolete. Instead, please use [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

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
### getName() {#getName--}
```
public String getName()
```


Gets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--).

**Remarks**

If this property is used to set the name of the font, the [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) will be updated to [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE)

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Gets the size of the font.

**Returns:**
int
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

Only for the fonts of Shapes or Charts. NOTE: This member is now obsolete. Instead, please use [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

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

**Remarks**

Only for the fonts of Shapes or Charts. NOTE: This member is now obsolete. Instead, please use [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Sets a value indicating whether the font is italic.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--).

**Remarks**

If this property is used to set the name of the font, the [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) will be updated to [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE)

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

Only for the fonts of Shapes or Charts. NOTE: This member is now obsolete. Instead, please use [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

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

