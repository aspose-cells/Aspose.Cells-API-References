---
title: "字体"
second_title: "Aspose.Cells for Java API 参考"
description: "封装在电子表格中使用的字体对象。"
type: docs
url: /zh/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

封装在电子表格中使用的字体对象。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | 检查两个字体是否相等。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | 获取具有 32 位 ARGB 值的颜色。 |
| [getCapsType()](#getCapsType--) | 获取文本大写类型。 |
| [getCharset()](#getCharset--) | 表示字符集。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 获取字体的 [Color](../../com.aspose.cells/color)。 |
| [getDoubleSize()](#getDoubleSize--) | 获取字体的双倍大小。 |
| [getName()](#getName--) | 获取 [Font](../../com.aspose.cells/font) 的名称。 |
| [getSchemeType()](#getSchemeType--) | 获取字体的方案类型。 |
| [getScriptOffset()](#getScriptOffset--) | 获取脚本偏移，以百分比为单位 |
| [getSize()](#getSize--) | 获取字体的大小。 |
| [getStrikeType()](#getStrikeType--) | 获取文本的删除线类型。 |
| [getThemeColor()](#getThemeColor--) | 获取主题颜色。 |
| [getUnderline()](#getUnderline--) | 获取字体的下划线类型。 |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | 获取指示字体是否加粗的值。 |
| [isItalic()](#isItalic--) | 获取指示字体是否斜体的值。 |
| [isNormalizeHeights()](#isNormalizeHeights--) | 指示是否对文本运行进行高度归一化。 |
| [isStrikeout()](#isStrikeout--) | 获取指示字体是否单一删除线的值。 |
| [isSubscript()](#isSubscript--) | 获取一个指示字体是否为下标的值。 |
| [isSuperscript()](#isSuperscript--) | 获取一个指示字体是否为上标的值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | 使用 32 位 ARGB 值设置颜色。 |
| [setBold(boolean value)](#setBold-boolean-) | 设置一个指示字体是否为粗体的值。 |
| [setCapsType(int value)](#setCapsType-int-) | 设置文本大写类型。 |
| [setCharset(int value)](#setCharset-int-) | 表示字符集。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 设置字体的[Color](../../com.aspose.cells/color)。 |
| [setDoubleSize(double value)](#setDoubleSize-double-) | 设置字体的双倍大小。 |
| [setItalic(boolean value)](#setItalic-boolean-) | 设置一个指示字体是否为斜体的值。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 [Font](../../com.aspose.cells/font) 的名称。 |
| [setName(String name, int type)](#setName-java.lang.String-int-) | 设置字体的名称和方案。 |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | 指示是否对文本运行进行高度归一化。 |
| [setSchemeType(int value)](#setSchemeType-int-) | 设置字体的方案类型。 |
| [setScriptOffset(double value)](#setScriptOffset-double-) | 设置脚本偏移量，单位为百分比。 |
| [setSize(int value)](#setSize-int-) | 设置字体的大小。 |
| [setStrikeType(int value)](#setStrikeType-int-) | 获取文本的删除线类型。 |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | 设置一个指示字体是否为单线删除线的值。 |
| [setSubscript(boolean value)](#setSubscript-boolean-) | 设置一个指示字体是否为下标的值。 |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | 设置一个指示字体是否为上标的值。 |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | 设置主题颜色。 |
| [setUnderline(int value)](#setUnderline-int-) | 设置字体的下划线类型。 |
| [toString()](#toString--) | 返回表示当前 Cell 对象的字符串。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


检查两个字体是否相等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | 比较字体对象。 |

**Returns:**
布尔值 - 如果等于比较的字体对象则为 True。
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


获取具有 32 位 ARGB 值的颜色。

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


获取文本大写类型。

参见[TextCapsType](../../com.aspose.cells/textcapstype)。

**Remarks**

仅适用于形状或图表的字体。注意：此成员已过时。请改用 [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) 属性。该属性将在自 2026 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


表示字符集。

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


获取字体的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


获取字体的双倍大小。

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


获取 [Font](../../com.aspose.cells/font) 的名称。

**Remarks**

如果使用此属性设置字体名称，则 [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) 将更新为 [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE)。

**Returns:**
java.lang.String
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


获取字体的方案类型。

参见[FontSchemeType](../../com.aspose.cells/fontschemetype)。

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


获取脚本偏移，以百分比为单位

**Remarks**

仅适用于形状和图表。

**Returns:**
double
### getSize() {#getSize--}
```
public int getSize()
```


获取字体的大小。

**Returns:**
int
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


获取文本的删除线类型。

参见[TextStrikeType](../../com.aspose.cells/textstriketype)。

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


获取主题颜色。

**Remarks**

如果字体颜色不是主题颜色，将返回 NULL。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


获取字体的下划线类型。

参见 [FontUnderlineType](../../com.aspose.cells/fontunderlinetype)。

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


获取指示字体是否加粗的值。

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


获取指示字体是否斜体的值。

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


指示是否对文本运行进行高度归一化。

**Remarks**

仅适用于形状或图表的字体。注意：此成员已过时。请改用 [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) 属性。该属性将在自 2026 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


获取指示字体是否单一删除线的值。

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


获取一个指示字体是否为下标的值。

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


获取一个指示字体是否为上标的值。

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


使用 32 位 ARGB 值设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


设置一个指示字体是否为粗体的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


设置文本大写类型。

参见[TextCapsType](../../com.aspose.cells/textcapstype)。

**Remarks**

仅适用于形状或图表的字体。注意：此成员已过时。请改用 [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--) 属性。该属性将在自 2026 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


表示字符集。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


设置字体的[Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


设置字体的双倍大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


设置一个指示字体是否为斜体的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置 [Font](../../com.aspose.cells/font) 的名称。

**Remarks**

如果使用此属性设置字体名称，则 [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) 将更新为 [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


设置字体的名称和方案。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype)。 |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


指示是否对文本运行进行高度归一化。

**Remarks**

仅适用于形状或图表的字体。注意：此成员已过时。请改用 [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--) 属性。该属性将在自 2026 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


设置字体的方案类型。

参见[FontSchemeType](../../com.aspose.cells/fontschemetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


设置脚本偏移量，单位为百分比。

**Remarks**

仅适用于形状和图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


设置字体的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


获取文本的删除线类型。

参见[TextStrikeType](../../com.aspose.cells/textstriketype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


设置一个指示字体是否为单线删除线的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


设置一个指示字体是否为下标的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


设置一个指示字体是否为上标的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


设置主题颜色。

**Remarks**

如果字体颜色不是主题颜色，将返回 NULL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


设置字体的下划线类型。

参见 [FontUnderlineType](../../com.aspose.cells/fontunderlinetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### toString() {#toString--}
```
public String toString()
```


返回表示当前 Cell 对象的字符串。

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

