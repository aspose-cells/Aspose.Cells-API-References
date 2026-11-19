---
title: "SplitPartInfo"
second_title: "Aspose.Cells for Java API 参考"
description: "表示多输入/输出中单个输入/输出的信息，例如在将电子表格转换为图像时要渲染的当前页面。"
type: docs
url: /zh/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

表示多输入/输出中单个输入/输出的信息，例如在将电子表格转换为图像时要渲染的当前页。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | 当前部分在序列中的索引（从 0 开始） |
| [getSheetIndex()](#getSheetIndex--) | 当前部分所在工作表的索引。-1 表示只有一个工作表。 |
| [getSheetName()](#getSheetName--) | 当前部分所在工作表的名称。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


当前部分在序列中的索引（从 0 开始）。-1 表示没有多个部分，因此结果为单一。

**Remarks**

如果需要处理多个工作表且每个工作表单独处理（拆分），则每个工作表的部分索引始终从 0 开始。例如，在将工作簿转换为图像时，它表示当前处理的工作表的输出页索引。-1 表示当前工作表只有一页。

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


当前部分所在工作表的索引。-1 表示只有一个工作表。

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


当前部分所在工作表的名称。

**Remarks**

在某些情况下可能为 null，例如在将整个工作簿渲染为 TIFF 图像时。

**Returns:**
java.lang.String
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

