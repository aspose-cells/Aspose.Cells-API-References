---
title: "DrawObjectEventHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "在渲染时获取 DrawObject 和 Bound 的接口。"
type: docs
url: /zh/java/com.aspose.cells/drawobjecteventhandler/
---

**Inheritance:**
java.lang.Object
```
public abstract class DrawObjectEventHandler
```

在渲染时获取 DrawObject 和 Bound 的接口。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DrawObjectEventHandler()](#DrawObjectEventHandler--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [draw(DrawObject drawObject, float x, float y, float width, float height)](#draw-com.aspose.cells.DrawObject-float-float-float-float-) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DrawObjectEventHandler() {#DrawObjectEventHandler--}
```
public DrawObjectEventHandler()
```


### draw(DrawObject drawObject, float x, float y, float width, float height) {#draw-com.aspose.cells.DrawObject-float-float-float-float-}
```
public void draw(DrawObject drawObject, float x, float y, float width, float height)
```


实现此接口以在渲染时获取 DrawObject 和 Bound。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| drawObject | [DrawObject](../../com.aspose.cells/drawobject) | 在渲染时将初始化并返回 DrawObject |
| x | float | DrawObject 的左侧 |
| y | float | DrawObject 的顶部 |
| 宽度 | float | DrawObject 的宽度 |
| 高度 | float | DrawObject 的高度 |

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

