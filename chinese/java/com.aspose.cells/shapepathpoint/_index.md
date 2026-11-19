---
title: "ShapePathPoint"
second_title: "Aspose.Cells for Java API 参考"
description: "指定位置坐标或角度标记。"
type: docs
url: /zh/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

指定位置坐标或角度标记。位置坐标表示坐标空间中路径的坐标（例如 X/Y）。角度标记指示路径中的角度变化（例如弧的起始角度和摆动角度）。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | 指定当前对象的值类型。 |
| [getX()](#getX--) | 获取此位置坐标的 X 坐标。 |
| [getXAngle()](#getXAngle--) | 当对象是角度标记时，获取或设置第一个角度（单位：度）。 |
| [getXPixel()](#getXPixel--) | 当对象是位置坐标时，获取或设置 X 坐标（单位：像素）。 |
| [getY()](#getY--) | 获取此位置坐标的 Y 坐标。 |
| [getYAngle()](#getYAngle--) | 当对象是角度标记时，获取或设置第二个角度（单位：度）。 |
| [getYPixel()](#getYPixel--) | 当对象是位置坐标时，获取或设置 Y 坐标（单位：像素）。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | 设置此位置坐标的 X 坐标。 |
| [setXAngle(int value)](#setXAngle-int-) | 当对象是角度标记时，获取或设置第一个角度（单位：度）。 |
| [setXPixel(int value)](#setXPixel-int-) | 当对象是位置坐标时，获取或设置 X 坐标（单位：像素）。 |
| [setY(int value)](#setY-int-) | 获取此位置坐标的 Y 坐标。 |
| [setYAngle(int value)](#setYAngle-int-) | 当对象是角度标记时，获取或设置第二个角度（单位：度）。 |
| [setYPixel(int value)](#setYPixel-int-) | 当对象是位置坐标时，获取或设置 Y 坐标（单位：像素）。 |
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
### getType() {#getType--}
```
public int getType()
```


指定当前对象的值类型。

参见 [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype)。

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


获取此位置坐标的 X 坐标。单位 EMU。

**Remarks**

注意：此成员已过时。请改用 ShapePathPoint.XPixel 和 ShapePathPoint.XAngle 属性。此属性将在自 2025 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


当对象是角度标记时，获取或设置第一个角度（单位：度）。

**Remarks**

如果此角度是弧的起始角度。该角度将指定在假想圆路径上用于绘制弧的起始位置的角度。此起始角度将锁定在形状路径中上一次已知的笔位置，从而保证连续的形状路径。

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


当对象是位置坐标时，获取或设置 X 坐标（单位：像素）。

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


获取此位置坐标的 Y 坐标。单位 EMU。

**Remarks**

注意：此成员已过时。请改用 ShapePathPoint.YPixel 和 ShapePathPoint.YAngle 属性。此属性将在自 2025 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


当对象是角度标记时，获取或设置第二个角度（单位：度）。

**Remarks**

如果此角度是弧的摆动角度。该角度将指定弧在假想圆路径上沿角度方向延伸的距离。相对于起始角度的延伸始终沿顺时针方向围绕假想圆进行。

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


当对象是位置坐标时，获取或设置 Y 坐标（单位：像素）。

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




### setX(int value) {#setX-int-}
```
public void setX(int value)
```


设置此位置坐标的 X 坐标。单位 EMU。

**Remarks**

注意：此成员已过时。请改用 ShapePathPoint.XPixel 和 ShapePathPoint.XAngle 属性。此属性将在自 2025 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


当对象是角度标记时，获取或设置第一个角度（单位：度）。

**Remarks**

如果此角度是弧的起始角度。该角度将指定在假想圆路径上用于绘制弧的起始位置的角度。此起始角度将锁定在形状路径中上一次已知的笔位置，从而保证连续的形状路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


当对象是位置坐标时，获取或设置 X 坐标（单位：像素）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


获取此位置坐标的 Y 坐标。单位 EMU。

**Remarks**

注意：此成员已过时。请改用 ShapePathPoint.YPixel 和 ShapePathPoint.YAngle 属性。此属性将在自 2025 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


当对象是角度标记时，获取或设置第二个角度（单位：度）。

**Remarks**

如果此角度是弧的摆动角度。该角度将指定弧在假想圆路径上沿角度方向延伸的距离。相对于起始角度的延伸始终沿顺时针方向围绕假想圆进行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


当对象是位置坐标时，获取或设置 Y 坐标（单位：像素）。

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

