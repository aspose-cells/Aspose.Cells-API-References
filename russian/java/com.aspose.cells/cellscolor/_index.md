---
title: "CellsColor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все типы цвета."
type: docs
url: /ru/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Представляет все типы цвета.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Получает цвет из 32‑битного значения ARGB. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Получает цвет RGB. |
| [getColorIndex()](#getColorIndex--) | Получает индекс цвета в палитре. |
| [getThemeColor()](#getThemeColor--) | Получает цвет темы. |
| [getTransparency()](#getTransparency--) | Получает прозрачность в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [getType()](#getType--) | Тип цвета. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Получает цвет, который должен применяться к ячейке или фигуре. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Устанавливает цвет из 32‑битного значения ARGB. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Устанавливает цвет RGB. |
| [setColorIndex(int value)](#setColorIndex-int-) | Устанавливает индекс цвета в палитре. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Устанавливает цвет, который должен применяться к ячейке или фигуре. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Получает цвет темы. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Установите оттенок цвета фигуры |
| [setTransparency(double value)](#setTransparency-double-) | Устанавливает прозрачность в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


Получает цвет из 32‑битного значения ARGB.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Получает цвет RGB.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Получает индекс цвета в палитре. Применяется только к индексированному цвету.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Получает цвет темы. Применяется только к типу цвета темы.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Получает прозрачность в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Тип цвета.

См. [ColorType](../../com.aspose.cells/colortype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


Получает цвет, который должен применяться к ячейке или фигуре.

**Remarks**

Выражение цвета ячейки и фигуры различается. Например, цвет темы с одинаковым значением оттенка будет различаться в ячейке и в фигуре.

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




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


Устанавливает цвет из 32‑битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Устанавливает цвет RGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Устанавливает индекс цвета в палитре. Применяется только к индексированному цвету.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Устанавливает цвет, который должен применяться к ячейке или фигуре.

**Remarks**

Выражение цвета ячейки и фигуры различается. Например, цвет темы с одинаковым значением оттенка будет различаться в ячейке и в фигуре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Получает цвет темы. Применяется только к типу цвета темы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Установите оттенок цвета фигуры

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Устанавливает прозрачность в виде значения от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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

