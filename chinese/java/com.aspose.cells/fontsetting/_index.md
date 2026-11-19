---
title: "FontSetting"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单元格文本中的字符范围。"
type: docs
url: /zh/java/com.aspose.cells/fontsetting/
---

**Inheritance:**
java.lang.Object
```
public class FontSetting
```

表示单元格文本中的字符范围。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         //getting characters
         FontSetting character = cell.characters(6, 7);
 
         //Setting the font of selected characters to bold
         character.getFont().setBold(true);
 
         //Setting the font color of selected characters to blue
         character.getFont().setColor(Color.getBlue());
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FontSetting(int startIndex, int length, WorksheetCollection sheets)](#FontSetting-int-int-com.aspose.cells.WorksheetCollection-) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | 返回此对象的字体。 |
| [getLength()](#getLength--) | 获取字符的长度。 |
| [getStartIndex()](#getStartIndex--) | 获取字符的起始索引。 |
| [getTextOptions()](#getTextOptions--) | 返回文本选项。 |
| [getType()](#getType--) | 获取文本节点的类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | 设置预设的 WordArt 样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontSetting(int startIndex, int length, WorksheetCollection sheets) {#FontSetting-int-int-com.aspose.cells.WorksheetCollection-}
```
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | [WorksheetCollection](../../com.aspose.cells/worksheetcollection) |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


返回此对象的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


获取字符的长度。

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


获取字符的起始索引。

**Returns:**
int
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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

