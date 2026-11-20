---
title: "ChartSplitType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет способ разделения двух секций либо диаграммы «круг в круге», либо диаграммы «бар в круге»."
type: docs
url: /ru/java/com.aspose.cells/chartsplittype/
---

**Inheritance:**
java.lang.Object
```
public final class ChartSplitType
```

Представляет способ разделения двух секций либо диаграммы «круг в круге», либо диаграммы «бар в круге».
## Поля

| Поле | Описание |
| --- | --- |
| [AUTO](#AUTO) | Представляет точки данных, которые должны быть разделены с использованием механизма по умолчанию для этого типа диаграммы. |
| [CUSTOM](#CUSTOM) | Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой в соответствии со значениями пользовательского разделения. |
| [PERCENT_VALUE](#PERCENT-VALUE) | Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой, помещая точки с процентом меньше значения Split Position в вторую диаграмму. |
| [POSITION](#POSITION) | Представляет точки данных. |
| [VALUE](#VALUE) | Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой, помещая точки данных со значением меньше Split Position во вторую диаграмму. |
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
### AUTO {#AUTO}
```
public static final int AUTO
```


Представляет точки данных, которые должны быть разделены с использованием механизма по умолчанию для этого типа диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Series.IsAutoSplit. Это свойство будет удалено через 12 месяцев, начиная с сентября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой в соответствии со значениями пользовательского разделения.

### PERCENT_VALUE {#PERCENT-VALUE}
```
public static final int PERCENT_VALUE
```


Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой, помещая точки с процентом меньше значения Split Position в вторую диаграмму.

### POSITION {#POSITION}
```
public static final int POSITION
```


Представляет точки данных. Точки данных должны быть разделены между круговой диаграммой и второй диаграммой, помещая последнюю позицию разделения точек данных во вторую диаграмму.

### VALUE {#VALUE}
```
public static final int VALUE
```


Представляет точки данных, которые должны быть разделены между круговой диаграммой и второй диаграммой, помещая точки данных со значением меньше Split Position во вторую диаграмму.

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

