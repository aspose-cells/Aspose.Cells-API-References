---
title: TextParagraph
second_title: Aspose.Cells for Java API Reference
description: Represents the text paragraph setting.
type: docs
weight: 580
url: /java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Represents the text paragraph setting.
## Constructors

| Constructor | Description |
| --- | --- |
| [TextParagraph()](#TextParagraph--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Gets and sets the text horizontal alignment type of the paragraph. |
| [getBullet()](#getBullet--) | Gets the bullet. |
| [getChildren()](#getChildren--) | Gets all text runs in this paragraph. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Gets and sets the default size for a tab character within this paragraph. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [getFont()](#getFont--) | Returns the font of this object. |
| [getFontAlignType()](#getFontAlignType--) | Determines where vertically on a line of text the actual words are positioned. |
| [getLeftMargin()](#getLeftMargin--) | Specifies the left margin of the paragraph. |
| [getLength()](#getLength--) | Gets the length of the characters. |
| [getLineSpace()](#getLineSpace--) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getRightMargin()](#getRightMargin--) | Specifies the right margin of the paragraph. |
| [getSpaceAfter()](#getSpaceAfter--) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceBefore()](#getSpaceBefore--) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getStartIndex()](#getStartIndex--) | Gets the start index of the characters. |
| [getStops()](#getStops--) | Gets tab stop list. |
| [getTextOptions()](#getTextOptions--) | Returns the text options. |
| [getType()](#getType--) | Gets the type of text node. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | For the description of this property, please see \#getAlignmentType().getAlignmentType() |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | For the description of this property, please see \#getDefaultTabSize().getDefaultTabSize() |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | For the description of this property, please see \#isEastAsianLineBreak().isEastAsianLineBreak() |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | For the description of this property, please see \#getFirstLineIndent().getFirstLineIndent() |
| [setFontAlignType(int value)](#setFontAlignType-int-) | For the description of this property, please see \#getFontAlignType().getFontAlignType() |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | For the description of this property, please see \#isHangingPunctuation().isHangingPunctuation() |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | For the description of this property, please see \#isLatinLineBreak().isLatinLineBreak() |
| [setLeftMargin(double value)](#setLeftMargin-double-) | For the description of this property, please see \#getLeftMargin().getLeftMargin() |
| [setLineSpace(double value)](#setLineSpace-double-) | For the description of this property, please see \#getLineSpace().getLineSpace() |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | For the description of this property, please see \#getLineSpaceSizeType().getLineSpaceSizeType() |
| [setRightMargin(double value)](#setRightMargin-double-) | For the description of this property, please see \#getRightMargin().getRightMargin() |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | For the description of this property, please see \#getSpaceAfter().getSpaceAfter() |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | For the description of this property, please see \#getSpaceAfterSizeType().getSpaceAfterSizeType() |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | For the description of this property, please see \#getSpaceBefore().getSpaceBefore() |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | For the description of this property, please see \#getSpaceBeforeSizeType().getSpaceBeforeSizeType() |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Sets the preset WordArt style. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TextParagraph() {#TextParagraph--}
```
public TextParagraph()
```


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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Gets and sets the text horizontal alignment type of the paragraph.

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Gets the bullet.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Gets and sets the default size for a tab character within this paragraph.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Specifies the indent size that will be applied to the first line of text in the paragraph.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Returns the font of this object.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines.

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Specifies the left margin of the paragraph.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Gets the length of the characters.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Gets and sets the amount of vertical white space that will be used within a paragraph.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Gets and sets the amount of vertical white space that will be used within a paragraph.

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Specifies the right margin of the paragraph.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Gets and sets the amount of vertical white space that will be present after a paragraph.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Gets and sets the amount of vertical white space that will be present after a paragraph.

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Gets and sets the amount of vertical white space that will be present before a paragraph.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Gets and sets the amount of vertical white space that will be present before a paragraph.

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Gets the start index of the characters.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Gets tab stop list.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Returns the text options.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Gets the type of text node.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


For the description of this property, please see \#getAlignmentType().getAlignmentType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


For the description of this property, please see \#getDefaultTabSize().getDefaultTabSize()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


For the description of this property, please see \#isEastAsianLineBreak().isEastAsianLineBreak()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


For the description of this property, please see \#getFirstLineIndent().getFirstLineIndent()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


For the description of this property, please see \#getFontAlignType().getFontAlignType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


For the description of this property, please see \#isHangingPunctuation().isHangingPunctuation()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


For the description of this property, please see \#isLatinLineBreak().isLatinLineBreak()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


For the description of this property, please see \#getLeftMargin().getLeftMargin()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


For the description of this property, please see \#getLineSpace().getLineSpace()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


For the description of this property, please see \#getLineSpaceSizeType().getLineSpaceSizeType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


For the description of this property, please see \#getRightMargin().getRightMargin()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


For the description of this property, please see \#getSpaceAfter().getSpaceAfter()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


For the description of this property, please see \#getSpaceAfterSizeType().getSpaceAfterSizeType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


For the description of this property, please see \#getSpaceBefore().getSpaceBefore()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


For the description of this property, please see \#getSpaceBeforeSizeType().getSpaceBeforeSizeType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Sets the preset WordArt style. Only for the text of shape/chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | int | The preset WordArt style. |

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

