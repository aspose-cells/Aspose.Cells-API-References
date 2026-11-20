---
title: "ShapePath"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые в совокупности образуют геометрическую форму."
type: docs
url: /ru/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые в совокупности образуют геометрическую форму.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ShapePath()](#ShapePath--) | Инициализирует новый экземпляр класса [ShapePath](../../com.aspose.cells/shapepath). |
## Методы

| Метод | Описание |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Добавляет эллиптическую дугу к текущей фигуре. |
| [close()](#close--) | Закрывает текущую фигуру и начинает новую фигуру. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Добавляет кубическую B\u8305zier кривую к текущей фигуре. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Получает высоту этого пути в пикселях. |
| [getPathSegementList()](#getPathSegementList--) | Получает список [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | Получает список [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | Получает ширину этого пути в пикселях. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Добавляет линейный сегмент к текущей фигуре. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Начинает новую фигуру из указанной точки, не закрывая текущую фигуру. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Получает высоту этого пути в пикселях. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Получает ширину этого пути в пикселях. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Инициализирует новый экземпляр класса [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Добавляет эллиптическую дугу к текущей фигуре. Начальная точка — конечная точка текущей фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| wR | float | Полуширина прямоугольной области \\u9225\\u5b27\\u20ac\\u5aa1he эллипса, рисующего дугу (Единица измерения: пиксель). |
| hR | float | Полувысота прямоугольной области \\u9225\\u5b27\\u20ac\\u5aa1he эллипса, рисующего дугу (Единица измерения: пиксель). |
| stAng | float | Начальный угол дуги, измеряемый в градусах по часовой стрелке от оси X (Единица измерения: градус). Этот угол указывает, какой угол вдоль предполагаемого пути окружности будет использоваться в качестве начальной позиции для рисования дуги. Этот начальный угол будет привязан к последнему известному положению пера в пути фигуры, тем самым гарантируя непрерывный путь фигуры. |
| swAng | float | Угол разворота дуги. Этот угол определяет, насколько далеко по углу вдоль предполагаемого пути круга будет расширяться дуга. Расширение от начального угла всегда будет происходить по часовой стрелке вокруг предполагаемого круга. (Единица измерения: градус) |

### close() {#close--}
```
public void close()
```


Закрывает текущую фигуру и начинает новую фигуру. Если текущая фигура содержит последовательность соединённых линий и кривых, метод замыкает контур, соединяя линию от конечной точки к начальной точке.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Добавляет кубическую B\\u8305zier кривую к текущей фигуре. Начальная точка — конечная точка текущей фигуры. Единица измерения: пиксель.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ctrX1 | float | Координата X первой контрольной точки кривой (Единица измерения: пиксель). |
| ctrY1 | float | Координата Y первой контрольной точки кривой (Единица измерения: пиксель). |
| ctrX2 | float | Координата X второй контрольной точки кривой (Единица измерения: пиксель). |
| ctrY2 | float | Координата Y второй контрольной точки кривой (Единица измерения: пиксель). |
| endX | float | Координата X конечной точки кривой (Единица измерения: пиксель). |
| endY | float | Координата Y конечной точки кривой (Единица измерения: пиксель). |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Получает высоту этого пути в пикселях.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Получает список [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ShapePath.PathSegments. Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Получает список [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Получает ширину этого пути в пикселях.

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


Добавляет линейный сегмент к текущей фигуре. Начальная точка — конечная точка текущей фигуры. Единица измерения: пиксель.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| x | float | Координата x конечной точки отрезка (Единица: Пиксель). |
| y | float | Координата y конечной точки отрезка (Единица: Пиксель). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Начинает новую фигуру из указанной точки без закрытия текущей фигуры. Все последующие точки, добавляемые в путь, добавляются в эту новую фигуру.Единица: Пиксель.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| x | float | Координата x начальной точки фигуры (Единица: Пиксель). |
| y | float | Координата y начальной точки фигуры (Единица: Пиксель). |

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


Получает высоту этого пути в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Получает ширину этого пути в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

