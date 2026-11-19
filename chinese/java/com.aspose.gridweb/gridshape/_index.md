---
title: "GridShape"
second_title: "Aspose.Cells for Java API 参考"
description: "表示形状对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

表示形状对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | 获取对象的缓冲区。 |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | 获取形状的 Sets ID。 |
| [getLeft()](#getLeft--) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [getLeftToCorner()](#getLeftToCorner--) | 表示形状相对于工作表左边界的水平偏移量，单位为像素。 |
| [getMsoDrawingType()](#getMsoDrawingType--) | 获取 mso 绘图类型。 |
| [getName()](#getName--) | 获取形状的名称。 |
| [getText()](#getText--) | 表示此 TextBox 对象中的字符串。 |
| [getTop()](#getTop--) | 表示形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [getTopToCorner()](#getTopToCorner--) | 表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。 |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | 表示左上角列索引。 |
| [getUpperLeftRow()](#getUpperLeftRow--) | 表示左上角行索引。 |
| [getZOrderPosition()](#getZOrderPosition--) | 返回形状在 Z 顺序中的位置。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | 创建图像并以指定的 png 格式保存到流中。 |
| [setID(String value)](#setID-java.lang.String-) | 获取形状的 Sets ID。 |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | 表示形状相对于工作表左边界的水平偏移量，单位为像素。 |
| [setText(String value)](#setText-java.lang.String-) | 表示此 TextBox 对象中的字符串。 |
| [setTopToCorner(int value)](#setTopToCorner-int-) | 表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。 |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | 返回形状在 Z 顺序中的位置。 |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


获取对象的缓冲区。

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


获取形状的 Sets ID。

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


表示形状相对于其左列的水平偏移，单位为像素。

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


表示形状相对于工作表左边界的水平偏移量，单位为像素。

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


获取 mso 绘图类型。

参见 [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype)。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取形状的名称。

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


表示此 TextBox 对象中的字符串。

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


表示形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

如果形状位于图表中，表示形状相对于其上边框的垂直偏移量。

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


表示左上角列索引。

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


表示左上角行索引。

**Remarks**

如果形状位于形状内部或组中，UpperLeftRow 将被忽略。

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


返回形状在 Z 顺序中的位置。

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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


创建图像并以指定的 png 格式保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


获取形状的 Sets ID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


表示形状相对于工作表左边界的水平偏移量，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


表示此 TextBox 对象中的字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


返回形状在 Z 顺序中的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

