---
title: Font
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the font object used in a spreadsheet.
type: docs
weight: 222
url: /java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Encapsulates the font object used in a spreadsheet.

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
| [getArgbColor()](#getArgbColor--) | Gets and sets the color with a 32-bit ARGB value. |
| [getCapsType()](#getCapsType--) | Gets and sets the text caps type. |
| [getCharset()](#getCharset--) | Represent the character set. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets or sets the [Color](../../com.aspose.cells/color) of the font. |
| [getDoubleSize()](#getDoubleSize--) | Gets and sets the double size of the font. |
| [getName()](#getName--) | Gets or sets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--). |
| [getSchemeType()](#getSchemeType--) | Gets and sets the scheme type of the font. |
| [getScriptOffset()](#getScriptOffset--) | Gets and sets the script offset,in unit of percentage |
| [getSize()](#getSize--) | Gets or sets the size of the font. |
| [getStrikeType()](#getStrikeType--) | Gets the strike type of the text. |
| [getThemeColor()](#getThemeColor--) | Gets and sets the theme color. |
| [getUnderline()](#getUnderline--) | Gets or sets the font underline type. |
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
| [setItalic(boolean value)](#setItalic-boolean-) | For the description of this property, please see \#isItalic().isItalic() |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see \#getName().getName() |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | For the description of this property, please see \#isNormalizeHeights().isNormalizeHeights() |
| [setSchemeType(int value)](#setSchemeType-int-) | For the description of this property, please see \#getSchemeType().getSchemeType() |
| [setScriptOffset(double value)](#setScriptOffset-double-) | For the description of this property, please see \#getScriptOffset().getScriptOffset() |
| [setSize(int value)](#setSize-int-) | For the description of this property, please see \#getSize().getSize() |
| [setStrikeType(int value)](#setStrikeType-int-) | For the description of this property, please see \#getStrikeType().getStrikeType() |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | For the description of this property, please see \#isStrikeout().isStrikeout() |
| [setSubscript(boolean value)](#setSubscript-boolean-) | For the description of this property, please see \#isSubscript().isSubscript() |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | For the description of this property, please see \#isSuperscript().isSuperscript() |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | For the description of this property, please see \#getThemeColor().getThemeColor() |
| [setUnderline(int value)](#setUnderline-int-) | For the description of this property, please see \#getUnderline().getUnderline() |
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
### getName() {#getName--}
```
public String getName()
```


Gets or sets the name of the [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--).

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Gets or sets the size of the font.

**Returns:**
int
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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


For the description of this property, please see \#isItalic().isItalic()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

