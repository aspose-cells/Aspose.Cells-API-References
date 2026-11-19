---
title: "TextParagraph"
second_title: "Aspose.Cells for Java API 参考"
description: "表示文本段落设置。"
type: docs
url: /zh/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

表示文本段落设置。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | 获取段落的文本水平对齐类型。 |
| [getBullet()](#getBullet--) | 获取项目符号。 |
| [getChildren()](#getChildren--) | 获取此段落中的所有文本运行。 |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | 获取此段落中制表符的默认大小。 |
| [getFirstLineIndent()](#getFirstLineIndent--) | 指定将在段落的第一行文本上应用的缩进大小。 |
| [getFont()](#getFont--) | 返回此对象的字体。 |
| [getFontAlignType()](#getFontAlignType--) | 确定文本行中实际单词的垂直位置。 |
| [getLeftMargin()](#getLeftMargin--) | 指定段落的左边距。 |
| [getLength()](#getLength--) | 获取字符的长度。 |
| [getLineSpace()](#getLineSpace--) | 获取段落内部使用的垂直空白量。 |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | 获取段落内部使用的垂直空白量。 |
| [getRightMargin()](#getRightMargin--) | 指定段落的右边距。 |
| [getSpaceAfter()](#getSpaceAfter--) | 获取段落后出现的垂直空白量。 |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | 获取段落后出现的垂直空白量。 |
| [getSpaceBefore()](#getSpaceBefore--) | 获取段落前出现的垂直空白量。 |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | 获取段落前出现的垂直空白量。 |
| [getStartIndex()](#getStartIndex--) | 获取字符的起始索引。 |
| [getStops()](#getStops--) | 获取制表位列表。 |
| [getTextOptions()](#getTextOptions--) | 返回文本选项。 |
| [getType()](#getType--) | 获取文本节点的类型。 |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | 指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。 |
| [isHangingPunctuation()](#isHangingPunctuation--) | 指定标点符号是强制布局在同一行文本上还是放在不同的行上。 |
| [isLatinLineBreak()](#isLatinLineBreak--) | 指定是否可以在不添加连字符的情况下将拉丁文字拆分并换行到下一行。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | 设置段落的文本水平对齐类型。 |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | 设置此段落中制表符的默认大小。 |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | 指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。 |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | 指定将在段落的第一行文本上应用的缩进大小。 |
| [setFontAlignType(int value)](#setFontAlignType-int-) | 确定文本行中实际单词的垂直位置。 |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | 指定标点符号是强制布局在同一行文本上还是放在不同的行上。 |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | 指定是否可以在不添加连字符的情况下将拉丁文字拆分并换行到下一行。 |
| [setLeftMargin(double value)](#setLeftMargin-double-) | 指定段落的左边距。 |
| [setLineSpace(double value)](#setLineSpace-double-) | 设置段落内部使用的垂直空白量。 |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | 设置段落内部使用的垂直空白量。 |
| [setRightMargin(double value)](#setRightMargin-double-) | 指定段落的右边距。 |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | 设置段落后出现的垂直空白量。 |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | 设置段落后出现的垂直空白量。 |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | 设置段落前出现的垂直空白量。 |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | 设置段落前出现的垂直空白量。 |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | 设置预设的 WordArt 样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


获取段落的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


获取项目符号。

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


获取此段落中的所有文本运行。如果此段落为空，返回段落本身。

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


获取此段落中制表符的默认大小。

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


指定将在段落的第一行文本上应用的缩进大小。

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


返回此对象的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


确定文本行中实际单词的垂直位置。这涉及字符相对于基线的垂直放置。

参见 [TextFontAlignType](../../com.aspose.cells/textfontaligntype)。

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


指定段落的左边距。

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


获取字符的长度。

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


获取段落内部使用的垂直空白量。

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


获取段落内部使用的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


指定段落的右边距。

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


获取段落后出现的垂直空白量。

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


获取段落后出现的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


获取段落前出现的垂直空白量。

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


获取段落前出现的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


获取字符的起始索引。

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


获取制表位列表。

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


返回文本选项。

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


获取文本节点的类型。

参见 [TextNodeType](../../com.aspose.cells/textnodetype).

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


指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


指定标点符号是强制布局在同一行文本上还是放在不同的行上。

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


指定是否可以在不添加连字符的情况下将拉丁文字拆分并换行到下一行。

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


设置段落的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


设置此段落中制表符的默认大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


指定将在段落的第一行文本上应用的缩进大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


确定文本行中实际单词的垂直位置。这涉及字符相对于基线的垂直放置。

参见 [TextFontAlignType](../../com.aspose.cells/textfontaligntype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


指定标点符号是强制布局在同一行文本上还是放在不同的行上。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


指定是否可以在不添加连字符的情况下将拉丁文字拆分并换行到下一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


指定段落的左边距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


设置段落内部使用的垂直空白量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


设置段落内部使用的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


指定段落的右边距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


设置段落后出现的垂直空白量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


设置段落后出现的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


设置段落前出现的垂直空白量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


设置段落前出现的垂直空白量。

参见 [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


设置预设的 WordArt 样式。

**Remarks**

仅适用于形状/图表的文本.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). 预设的 WordArt 样式. |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

