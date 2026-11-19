---
title: "SheetSet"
second_title: "Aspose.Cells for Java API 参考"
description: "描述一组工作表。"
type: docs
url: /zh/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

描述一组工作表。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | 基于精确的工作表索引创建工作表集合。 |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | 基于精确的工作表名称创建工作表集合。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | 获取包含工作簿活动工作表的集合。 |
| [getAll()](#getAll--) | 获取包含工作簿中所有工作表（按原始顺序）的集合。 |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | 获取包含工作簿中可见工作表（按原始顺序）的集合。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


基于精确的工作表索引创建工作表集合。

**Remarks**

如果遇到工作表不在工作簿中，将在渲染期间抛出异常。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndexes | int[] | 零基工作表索引。 |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


基于精确的工作表名称创建工作表集合。

**Remarks**

如果遇到工作表不在工作簿中，将在渲染期间抛出异常。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetNames | java.lang.String[] | 工作表名称。 |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


获取包含工作簿活动工作表的集合。

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


获取包含工作簿中所有工作表（按原始顺序）的集合。

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


获取包含工作簿中可见工作表（按原始顺序）的集合。

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

