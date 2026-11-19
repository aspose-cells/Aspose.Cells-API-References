---
title: "ShapePath"
second_title: "Aspose.Cells for Java API 参考"
description: "表示一个创建路径，由一系列移动、直线和曲线组成，组合后形成几何形状。"
type: docs
url: /zh/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

表示由一系列移动、直线和曲线组成的创建路径，组合后形成几何形状。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ShapePath()](#ShapePath--) | 初始化 [ShapePath](../../com.aspose.cells/shapepath) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | 向当前图形追加椭圆弧。 |
| [close()](#close--) | 关闭当前图形并开始新图形。 |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | 向当前图形追加三次 B\u8305zier 曲线。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | 获取此路径的高度，单位为像素。 |
| [getPathSegementList()](#getPathSegementList--) | 获取 [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) 列表 |
| [getPathSegments()](#getPathSegments--) | 获取 [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) 列表 |
| [getWidthPixel()](#getWidthPixel--) | 获取此路径的宽度，单位为像素。 |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | 向当前图形追加线段。 |
| [moveTo(float x, float y)](#moveTo-float-float-) | 从指定点开始新图形，而不关闭当前图形。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | 获取此路径的高度，单位为像素。 |
| [setWidthPixel(int value)](#setWidthPixel-int-) | 获取此路径的宽度，单位为像素。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


初始化 [ShapePath](../../com.aspose.cells/shapepath) 类的新实例。

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


向当前图形追加椭圆弧。起始点是当前图形的结束点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| wR | float | 绘制弧线的椭圆的矩形区域的半宽度（单位：像素）。 |
| hR | float | 绘制弧线的椭圆的矩形区域的半高度（单位：像素）。 |
| stAng | float | 弧线的起始角度，以度为单位，顺时针从 x 轴测量（单位：度）。该角度指定在假想的圆路径上用于绘制弧线的起始位置。此起始角度将锁定到形状路径中上一次已知的笔位置，从而保证连续的形状路径。 |
| swAng | float | 弧线的摆动角度。该角度指定沿假想圆路径的角度范围，弧线将被延伸的程度。延伸将始终从起始角度以顺时针方向围绕假想圆进行。（单位：度） |

### close() {#close--}
```
public void close()
```


关闭当前图形并开始一个新图形。如果当前图形包含一系列相连的直线和曲线，方法通过将一条线从端点连接到起点来闭合循环。

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


向当前图形追加一个三次 B\u8305zier 曲线。起始点是当前图形的终点。单位：像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ctrX1 | float | 曲线第一个控制点的 x 坐标（单位：像素）。 |
| ctrY1 | float | 曲线第一个控制点的 y 坐标（单位：像素）。 |
| ctrX2 | float | 曲线第二个控制点的 x 坐标（单位：像素）。 |
| ctrY2 | float | 曲线第二个控制点的 y 坐标（单位：像素）。 |
| endX | float | 曲线终点的 x 坐标（单位：像素）。 |
| endY | float | 曲线终点的 y 坐标（单位：像素）。 |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


获取此路径的高度，单位为像素。

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


获取 [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) 列表

**Remarks**

注意：此成员已过时。请改用 **ShapePath.PathSegments** 属性。此属性将在自 2026 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


获取 [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) 列表

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


获取此路径的宽度，单位为像素。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```


向当前图形追加一条线段。起始点是当前图形的终点。单位：像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| x | float | 线段终点的 x 坐标（单位：像素）。 |
| y | float | 线段终点的 y 坐标（单位：像素）。 |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


从指定点开始一个新图形而不关闭当前图形。随后添加到路径的所有点都将添加到此新图形。单位：像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| x | float | 图形起始点的 x 坐标（单位：像素）。 |
| y | float | 图形起始点的 y 坐标（单位：像素）。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


获取此路径的高度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


获取此路径的宽度，单位为像素。

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

