---
title: "名称"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单元格范围的已定义名称。"
type: docs
url: /zh/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

表示单元格范围的已定义名称。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | 获取名称的注释。 |
| [getFullText()](#getFullText--) | 获取具有作用域设置的对象的名称完整文本。 |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | 获取 [Name](../../com.aspose.cells/name) 的 R1C1 引用。 |
| [getRange()](#getRange--) | 如果此名称引用了范围，则获取该范围。 |
| [getRange(boolean recalculate)](#getRange-boolean-) | 如果此名称引用了范围，则获取该范围 |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | 如果此名称引用了范围，则获取该范围。 |
| [getRanges()](#getRanges--) | 获取此名称引用的所有范围。 |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | 获取此名称引用的所有范围。 |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | 获取此名称引用的所有引用。 |
| [getRefersTo()](#getRefersTo--) | 返回或设置名称定义引用的公式，公式以等号开头。 |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | 获取此 Name 的引用。 |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | 根据指定单元格获取此 Name 的引用。 |
| [getSheetIndex()](#getSheetIndex--) | 指示此名称属于工作簿或工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。 |
| [getText()](#getText--) | 获取对象的名称文本。 |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | 指示此名称是否被其他公式引用。 |
| [isVisible()](#isVisible--) | 指示名称是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | 设置名称的注释。 |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | 设置 [Name](../../com.aspose.cells/name) 的 R1C1 引用。 |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | 返回或设置名称定义引用的公式，公式以等号开头。 |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | 设置此 Name 的引用。 |
| [setSheetIndex(int value)](#setSheetIndex-int-) | 指示此名称属于工作簿或工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。 |
| [setText(String value)](#setText-java.lang.String-) | 获取对象的名称文本。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示名称是否可见。 |
| [toString()](#toString--) | 返回表示当前 Range 对象的字符串。 |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


获取名称的注释。仅适用于 Excel 2007 或更高版本。

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


获取具有作用域设置的对象的名称完整文本。

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


获取 [Name](../../com.aspose.cells/name) 的 R1C1 引用。

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


如果此名称引用了范围，则获取该范围。

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


如果此名称引用了范围，则获取该范围

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 重新计算 | boolean | 如果此名称在本次调用之前已经计算过，是否重新计算它。 |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


如果此名称引用的是范围，则获取该范围。如果此名称的引用不是绝对的，则对于不同的单元格范围可能不同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 相应的工作表索引。 |
| 行 | int | 相应的行索引。 |
| 列 | int | 相应的列索引 |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


获取此名称引用的所有范围。

**Returns:**
com.aspose.cells.Range[] - 所有范围。
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


获取此名称引用的所有范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 重新计算 | boolean | 如果此名称在本次调用之前已经计算过，是否重新计算它。 |

**Returns:**
com.aspose.cells.Range[] - 所有范围。
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


获取此名称引用的所有引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 重新计算 | boolean | 如果此名称在本次调用之前已经计算过，是否重新计算它。 |

**Returns:**
com.aspose.cells.ReferredArea[] - 所有范围。
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


返回或设置名称定义引用的公式，公式以等号开头。

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


获取此 Name 的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 引用是否需要格式化为 R1C1。 |
| isLocal | boolean | 引用是否需要按区域设置格式化。 |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


根据指定单元格获取此 Name 的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 引用是否需要格式化为 R1C1。 |
| isLocal | boolean | 引用是否需要按区域设置格式化。 |
| 行 | int | 单元格的行索引。 |
| 列 | int | 单元格的列索引。 |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


指示此名称属于工作簿或工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


获取对象的名称文本。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


指示此名称是否被其他公式引用。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


指示名称是否可见。

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


设置名称的注释。仅适用于 Excel 2007 或更高版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


设置 [Name](../../com.aspose.cells/name) 的 R1C1 引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


返回或设置名称定义引用的公式，公式以等号开头。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


设置此 Name 的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| refersTo | java.lang.String | 引用。 |
| isR1C1 | boolean | 引用是否为 R1C1 格式。 |
| isLocal | boolean | 引用是否已按区域设置格式化。 |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


指示此名称属于工作簿或工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


获取对象的名称文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示名称是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### toString() {#toString--}
```
public String toString()
```


返回表示当前 Range 对象的字符串。

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

