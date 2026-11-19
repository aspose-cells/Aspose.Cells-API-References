---
title: "DeleteBlankOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示删除空单元格/行/列的设置。"
type: docs
url: /zh/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

表示删除空单元格/行/列的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | 指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。 |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | 当单元格为公式且计算结果为 null 或空字符串时，是否将该单元格视为空白。 |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | 当单元格的值为空字符串时，是否将其视为空白。 |
| [getEndIndex()](#getEndIndex--) | 指定要检查并删除空白行/列的范围的结束行/列索引（含）。 |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | 获取用于跟踪删除导致的更改的监视器。 |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | 指示在删除空白行/列时如何处理合并单元格。 |
| [getStartIndex()](#getStartIndex--) | 指定要检查并删除空白行/列的范围的起始行/列索引。 |
| [getUpdateReference()](#getUpdateReference--) | 指示是否更新其他工作表中的引用。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | 指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。 |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | 当单元格为公式且计算结果为 null 或空字符串时，是否将该单元格视为空白。 |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | 当单元格的值为空字符串时，是否将其视为空白。 |
| [setEndIndex(int value)](#setEndIndex-int-) | 指定要检查并删除空白行/列的范围的结束行/列索引（含）。 |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | 设置用于跟踪删除导致的更改的监视器。 |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | 指示在删除空白行/列时如何处理合并单元格。 |
| [setStartIndex(int value)](#setStartIndex-int-) | 指定要检查并删除空白行/列的范围的起始行/列索引。 |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | 指示是否更新其他工作表中的引用。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。默认值为 true。

**Remarks**

当将此属性设置为 false 时，所有被绘图对象覆盖的行/列将不被视为空白，也不会被删除。

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


当单元格为公式且计算结果为 null 或空字符串时，是否将其视为空白。默认值为 false。

**Remarks**

通常用户应确保在将此属性设为 true 并执行删除操作之前已计算公式。否则，通过普通 API（如 [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)）新创建的所有公式将被视为空白并可能被删除，因为在计算之前它们的计算结果均为 null。

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


当单元格的值为空字符串时，是否将其视为空白。默认值为 true。

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


指定要检查并删除空白行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、绘图等）的最大范围。

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


获取用于跟踪删除导致的更改的监视器。

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


指示在删除空白行/列时如何处理合并单元格。

参见 [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype)。

**Remarks**

对于 [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY)，其中的所有单元格都将被视为空白，除非是非空的左上角单元格。这是此属性的默认值。

对于 [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE)，其中的所有单元格都将被视为非空白。

对于 [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT)，内容显示区域之外的所有单元格都将被视为空白。



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


指定要检查并删除空白行/列的范围的起始行/列索引。

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


指示是否更新其他工作表中的引用。

**Remarks**

从 26.7 开始，我们将此属性的默认值设为 true。

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


指示诸如图片、形状、图表等绘图相关对象是否将被视为空白。默认值为 true。

**Remarks**

当将此属性设置为 false 时，所有被绘图对象覆盖的行/列将不被视为空白，也不会被删除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


当单元格为公式且计算结果为 null 或空字符串时，是否将其视为空白。默认值为 false。

**Remarks**

通常用户应确保在将此属性设为 true 并执行删除操作之前已计算公式。否则，通过普通 API（如 [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)）新创建的所有公式将被视为空白并可能被删除，因为在计算之前它们的计算结果均为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


当单元格的值为空字符串时，是否将其视为空白。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


指定要检查并删除空白行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、绘图等）的最大范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


设置用于跟踪删除导致的更改的监视器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


指示在删除空白行/列时如何处理合并单元格。

参见 [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype)。

**Remarks**

对于 [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY)，其中的所有单元格都将被视为空白，除非是非空的左上角单元格。这是此属性的默认值。

对于 [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE)，其中的所有单元格都将被视为非空白。

对于 [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT)，内容显示区域之外的所有单元格都将被视为空白。



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


指定要检查并删除空白行/列的范围的起始行/列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


指示是否更新其他工作表中的引用。

**Remarks**

从 26.7 开始，我们将此属性的默认值设为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

