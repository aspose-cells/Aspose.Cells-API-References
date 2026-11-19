---
title: "SetBorderPosition"
second_title: "Aspose.Cells for Java API 参考"
description: "表示要设置的单元格范围的边框位置。"
type: docs
url: /zh/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

表示要设置的单元格范围的边框位置。

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## 字段

| 字段 | 描述 |
| --- | --- |
| [BOTTOM](#BOTTOM) | 底部边框 |
| [CROSS](#CROSS) | 交叉边框 |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | 底部边框 |
| [LEFT](#LEFT) | 左侧边框 |
| [NONE](#NONE) | 无边框 |
| [OUTLINE](#OUTLINE) | 垂直中间边框 |
| [RIGHT](#RIGHT) | 右侧边框 |
| [TOP](#TOP) | 顶部边框 |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | 水平中间边框 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```


底部边框

### CROSS {#CROSS}
```
public static final int CROSS
```


交叉边框

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


底部边框

### LEFT {#LEFT}
```
public static final int LEFT
```


左侧边框

### NONE {#NONE}
```
public static final int NONE
```


无边框

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


垂直中间边框

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


右侧边框

### TOP {#TOP}
```
public static final int TOP
```


顶部边框

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


水平中间边框

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

