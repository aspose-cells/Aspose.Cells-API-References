---
title: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Java API 参考"
description: "PdfBookmarkEntry 是 PDF 书签中的条目。"
type: docs
url: /zh/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry 是 PDF 书签中的一个条目。如果当前实例的 Text 属性为 null 或 ""，则该实例将被隐藏，子项将插入到当前层级。

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add();
         workbook.getWorksheets().add();
         Cell cellInPage1 = workbook.getWorksheets().get(0).getCells().get("A1");
         Cell cellInPage2 = workbook.getWorksheets().get(1).getCells().get("A1");
         Cell cellInPage3 = workbook.getWorksheets().get(2).getCells().get("A1");
         cellInPage1.putValue("page1");
         cellInPage2.putValue("page2");
         cellInPage3.putValue("page3");
 
         PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
         pbeRoot.setText("root");  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
         pbeRoot.setDestination(cellInPage1);
         pbeRoot.setSubEntry(new ArrayList());
         pbeRoot.setOpen(false);
 
         PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
         subPbe1.setText("section1");
         subPbe1.setDestination(cellInPage2);
 
         PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
         subPbe2.setText("section2");
         subPbe2.setDestination(cellInPage3);
 
         pbeRoot.getSubEntry().add(subPbe1);
         pbeRoot.getSubEntry().add(subPbe2);
 
         PdfSaveOptions saveOptions = new PdfSaveOptions();
         saveOptions.setBookmark(pbeRoot);
         workbook.save("output_bookmark.pdf", saveOptions);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | 书签链接指向的单元格。 |
| [getDestinationName()](#getDestinationName--) | 获取目标名称。 |
| [getSubEntry()](#getSubEntry--) | 书签的子条目。 |
| [getText()](#getText--) | 书签的标题。 |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | 当此属性为 true 时，书签条目将折叠，否则将展开。 |
| [isOpen()](#isOpen--) | 当此属性为 true 时，书签条目将展开，否则将折叠。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | 当此属性为 true 时，书签条目将折叠，否则将展开。 |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | 书签链接指向的单元格。 |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | 设置目标名称。 |
| [setOpen(boolean value)](#setOpen-boolean-) | 当此属性为 true 时，书签条目将展开，否则将折叠。 |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | 书签的子条目。 |
| [setText(String value)](#setText-java.lang.String-) | 书签的标题。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfBookmarkEntry() {#PdfBookmarkEntry--}
```
public PdfBookmarkEntry()
```


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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


书签链接指向的单元格。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


获取目标名称。

**Remarks**

如果设置了目标名称，则该目标将被定义为具有此名称的命名目标。

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


书签的子条目。

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


书签的标题。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapse() {#isCollapse--}
```
public boolean isCollapse()
```


当此属性为 true 时，书签条目将折叠，否则将展开。

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


当此属性为 true 时，书签条目将展开，否则将折叠。

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




### setCollapse(boolean value) {#setCollapse-boolean-}
```
public void setCollapse(boolean value)
```


当此属性为 true 时，书签条目将折叠，否则将展开。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


书签链接指向的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


设置目标名称。

**Remarks**

如果设置了目标名称，则该目标将被定义为具有此名称的命名目标。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


当此属性为 true 时，书签条目将展开，否则将折叠。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


书签的子条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


书签的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

