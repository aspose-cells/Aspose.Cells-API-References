---
title: "DrawObject"
second_title: "Aspose.Cells for Java API 参考"
description: "在渲染时将初始化并返回 DrawObject。"
type: docs
url: /zh/java/com.aspose.cells/drawobject/
---

**Inheritance:**
java.lang.Object
```
public class DrawObject
```

在渲染时将初始化并返回 DrawObject。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | 指示渲染时的 Cell 对象。 |
| [getClass()](#getClass--) |  |
| [getCurrentPage()](#getCurrentPage--) | 指示 DrawObject 的页面索引。 |
| [getImageBytes()](#getImageBytes--) | 指示渲染时 Chart、Shape 的图像字节。 |
| [getShape()](#getShape--) | 指示渲染时的 Shape 对象。 |
| [getSheetIndex()](#getSheetIndex--) | 指示 DrawObject 的当前工作表索引。 |
| [getTotalPages()](#getTotalPages--) | 指示当前渲染中的总页数。 |
| [getType()](#getType--) | 指示 DrawObject 的类型。 |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


指示渲染时的 Cell 对象。可以访问单元格的所有属性。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPage() {#getCurrentPage--}
```
public int getCurrentPage()
```


指示 DrawObject 的页面索引。页面索引从零开始。一个工作表在渲染时包含多个页面。

**Returns:**
int
### getImageBytes() {#getImageBytes--}
```
public byte[] getImageBytes()
```


指示渲染时 Chart、Shape 的图像字节。

**Returns:**
byte[]
### getShape() {#getShape--}
```
public Shape getShape()
```


指示渲染时的 Shape 对象。可以访问形状的所有属性。

**Returns:**
[Shape](../../com.aspose.cells/shape)
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


指示 DrawObject 的当前工作表索引。

**Returns:**
int
### getTotalPages() {#getTotalPages--}
```
public int getTotalPages()
```


指示当前渲染中的总页数。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


指示 DrawObject 的类型。

参见 [DrawObjectEnum](../../com.aspose.cells/drawobjectenum)。

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

