---
title: "SetBorderPosition"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет позицию границы, которую следует установить для диапазона ячеек."
type: docs
url: /ru/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Представляет позицию границы, которую следует установить для диапазона ячеек.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Поля

| Поле | Описание |
| --- | --- |
| [BOTTOM](#BOTTOM) | Нижняя граница |
| [CROSS](#CROSS) | Перекрёстные границы |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Нижняя граница |
| [LEFT](#LEFT) | Левая граница |
| [NONE](#NONE) | Нет границ |
| [OUTLINE](#OUTLINE) | Границы вертикального центра |
| [RIGHT](#RIGHT) | Правая граница |
| [TOP](#TOP) | Верхняя граница |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | Границы горизонтального центра |
## Методы

| Метод | Описание |
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


Нижняя граница

### CROSS {#CROSS}
```
public static final int CROSS
```


Перекрёстные границы

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Нижняя граница

### LEFT {#LEFT}
```
public static final int LEFT
```


Левая граница

### NONE {#NONE}
```
public static final int NONE
```


Нет границ

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


Границы вертикального центра

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Правая граница

### TOP {#TOP}
```
public static final int TOP
```


Верхняя граница

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


Границы горизонтального центра

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

