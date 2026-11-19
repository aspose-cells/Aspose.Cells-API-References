---
title: "VerticalPageBreak"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示垂直分页符的对象。"
type: docs
url: /zh/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

封装表示垂直分页符的对象。

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取垂直分页符的列索引。 |
| [getEndRow()](#getEndRow--) | 获取垂直分页符的结束行索引。 |
| [getStartRow()](#getStartRow--) | 获取垂直分页符的起始行索引。 |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取垂直分页符的列索引。

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


获取垂直分页符的结束行索引。

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


获取垂直分页符的起始行索引。

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

