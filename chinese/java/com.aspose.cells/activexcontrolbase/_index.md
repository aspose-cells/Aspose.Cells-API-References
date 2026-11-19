---
title: "ActiveXControlBase"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 ActiveX 控件。"
type: docs
url: /zh/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

表示 ActiveX 控件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | 获取背景的 ole 颜色。 |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | 获取控件的二进制数据。 |
| [getForeOleColor()](#getForeOleColor--) | 获取前景的 OLE 颜色。 |
| [getHeight()](#getHeight--) | 获取控件的高度（单位为点）。 |
| [getLinkedCell()](#getLinkedCell--) | 获取链接的单元格。 |
| [getListFillRange()](#getListFillRange--) | 获取列表填充范围。 |
| [getMouseIcon()](#getMouseIcon--) | 获取用于在控件上显示为鼠标指针的自定义图标。 |
| [getMousePointer()](#getMousePointer--) | 获取在控件上显示为鼠标指针的图标类型。 |
| [getShadow()](#getShadow--) | 指示是否显示阴影。 |
| [getType()](#getType--) | 获取 ActiveX 控件的类型。 |
| [getWidth()](#getWidth--) | 获取控件的宽度（单位为点）。 |
| [getWorkbook()](#getWorkbook--) | 获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | 指示此控件是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setForeOleColor(int value)](#setForeOleColor-int-) | 设置前景的 OLE 颜色。 |
| [setHeight(double value)](#setHeight-double-) | 设置控件的高度（单位为点）。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置链接的单元格。 |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | 设置列表填充范围。 |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | 设置自定义图标，以在控件上显示为鼠标指针。 |
| [setMousePointer(int value)](#setMousePointer-int-) | 设置在控件上显示为鼠标指针的图标类型。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 指示是否显示阴影。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此控件是否可见。 |
| [setWidth(double value)](#setWidth-double-) | 以点为单位设置控件的宽度。 |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


获取背景的 ole 颜色。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


获取控件的二进制数据。

**Returns:**
byte[]
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


获取前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取控件的高度（单位为点）。

**Returns:**
double
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


获取链接的单元格。

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


获取列表填充范围。

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


获取用于在控件上显示为鼠标指针的自定义图标。

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


获取在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


指示是否显示阴影。

**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
```


获取 ActiveX 控件的类型。

参见 [ControlType](../../com.aspose.cells/controltype)。

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


获取控件的宽度（单位为点）。

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


指示此控件是否可见。

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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


设置背景的 OLE 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


设置前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


设置控件的高度（单位为点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


设置链接的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


设置列表填充范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


设置自定义图标，以在控件上显示为鼠标指针。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


设置在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


指示是否显示阴影。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示此控件是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


以点为单位设置控件的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

