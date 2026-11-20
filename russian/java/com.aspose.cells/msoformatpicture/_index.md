---
title: "MsoFormatPicture"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет формат изображения."
type: docs
url: /ru/java/com.aspose.cells/msoformatpicture/
---

**Inheritance:**
java.lang.Object
```
public class MsoFormatPicture
```

Представляет формат изображения.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomCrop()](#getBottomCrop--) | Представляет положение нижней границы области обрезки, выраженное в виде отношения к высоте изображения. |
| [getBottomCropInch()](#getBottomCropInch--) | Представляет положение нижней границы области обрезки, выраженное в дюймах. |
| [getBrightness()](#getBrightness--) | Представляет изменение яркости изображения в процентах. |
| [getClass()](#getClass--) |  |
| [getContrast()](#getContrast--) | Представляет изменение контрастности изображения в процентах. |
| [getGamma()](#getGamma--) | Представляет гамму изображения. |
| [getLeftCrop()](#getLeftCrop--) | Представляет положение левой границы области обрезки, выраженное в виде отношения к ширине изображения. |
| [getLeftCropInch()](#getLeftCropInch--) | Представляет положение левой границы области обрезки, выраженное в дюймах. |
| [getRightCrop()](#getRightCrop--) | Представляет положение правой границы области обрезки, выраженное в виде отношения к ширине изображения. |
| [getRightCropInch()](#getRightCropInch--) | Представляет положение правой границы области обрезки, выраженное в дюймах. |
| [getTopCrop()](#getTopCrop--) | Представляет положение верхней границы области обрезки, выраженное в виде отношения к высоте изображения. |
| [getTopCropInch()](#getTopCropInch--) | Представляет положение верхней границы области обрезки, выраженное в дюймах. |
| [getTransparency()](#getTransparency--) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [getTransparentColor()](#getTransparentColor--) | Получает прозрачный цвет изображения. |
| [hashCode()](#hashCode--) | Получает хеш-код. |
| [isBiLevel()](#isBiLevel--) | Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме. |
| [isGray()](#isGray--) | Указывает, должно ли это изображение отображаться в градациях серого. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBiLevel(boolean value)](#setBiLevel-boolean-) | Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме. |
| [setBottomCrop(double value)](#setBottomCrop-double-) | Представляет положение нижней границы области обрезки, выраженное в виде отношения к высоте изображения. |
| [setBottomCropInch(double value)](#setBottomCropInch-double-) | Представляет положение нижней границы области обрезки, выраженное в дюймах. |
| [setBrightness(double value)](#setBrightness-double-) | Представляет изменение яркости изображения в процентах. |
| [setContrast(double value)](#setContrast-double-) | Представляет изменение контрастности изображения в процентах. |
| [setGamma(double value)](#setGamma-double-) | Представляет гамму изображения. |
| [setGray(boolean value)](#setGray-boolean-) | Указывает, должно ли это изображение отображаться в градациях серого. |
| [setLeftCrop(double value)](#setLeftCrop-double-) | Представляет положение левой границы области обрезки, выраженное в виде отношения к ширине изображения. |
| [setLeftCropInch(double value)](#setLeftCropInch-double-) | Представляет положение левой границы области обрезки, выраженное в дюймах. |
| [setRightCrop(double value)](#setRightCrop-double-) | Представляет положение правой границы области обрезки, выраженное в виде отношения к ширине изображения. |
| [setRightCropInch(double value)](#setRightCropInch-double-) | Представляет положение правой границы области обрезки, выраженное в дюймах. |
| [setTopCrop(double value)](#setTopCrop-double-) | Представляет положение верхней границы области обрезки, выраженное в виде отношения к высоте изображения. |
| [setTopCropInch(double value)](#setTopCropInch-double-) | Представляет положение верхней границы области обрезки, выраженное в дюймах. |
| [setTransparency(double value)](#setTransparency-double-) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [setTransparentColor(CellsColor value)](#setTransparentColor-com.aspose.cells.CellsColor-) | Устанавливает прозрачный цвет изображения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomCrop() {#getBottomCrop--}
```
public double getBottomCrop()
```


Представляет положение нижней границы области обрезки, выраженное в виде отношения к высоте изображения.

**Returns:**
double
### getBottomCropInch() {#getBottomCropInch--}
```
public double getBottomCropInch()
```


Представляет положение нижней границы области обрезки, выраженное в дюймах.

**Returns:**
double
### getBrightness() {#getBrightness--}
```
public double getBrightness()
```


Представляет изменение яркости изображения в процентах.

**Remarks**

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getContrast() {#getContrast--}
```
public double getContrast()
```


Представляет изменение контрастности изображения в процентах.

**Remarks**

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

**Returns:**
double
### getGamma() {#getGamma--}
```
public double getGamma()
```


Представляет гамму изображения.

**Returns:**
double
### getLeftCrop() {#getLeftCrop--}
```
public double getLeftCrop()
```


Представляет положение левой границы области обрезки, выраженное в виде отношения к ширине изображения.

**Returns:**
double
### getLeftCropInch() {#getLeftCropInch--}
```
public double getLeftCropInch()
```


Представляет положение левой границы области обрезки, выраженное в дюймах.

**Returns:**
double
### getRightCrop() {#getRightCrop--}
```
public double getRightCrop()
```


Представляет положение правой границы области обрезки, выраженное в виде отношения к ширине изображения.

**Returns:**
double
### getRightCropInch() {#getRightCropInch--}
```
public double getRightCropInch()
```


Представляет положение правой границы области обрезки, выраженное в дюймах.

**Returns:**
double
### getTopCrop() {#getTopCrop--}
```
public double getTopCrop()
```


Представляет положение верхней границы области обрезки, выраженное в виде отношения к высоте изображения.

**Returns:**
double
### getTopCropInch() {#getTopCropInch--}
```
public double getTopCropInch()
```


Представляет положение верхней границы области обрезки, выраженное в дюймах.

**Returns:**
double
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Returns:**
double
### getTransparentColor() {#getTransparentColor--}
```
public CellsColor getTransparentColor()
```


Получает прозрачный цвет изображения.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public int hashCode()
```


Получает хеш-код.

**Returns:**
int -
### isBiLevel() {#isBiLevel--}
```
public boolean isBiLevel()
```


Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме.

**Returns:**
boolean
### isGray() {#isGray--}
```
public boolean isGray()
```


Указывает, должно ли это изображение отображаться в градациях серого.

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




### setBiLevel(boolean value) {#setBiLevel-boolean-}
```
public void setBiLevel(boolean value)
```


Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBottomCrop(double value) {#setBottomCrop-double-}
```
public void setBottomCrop(double value)
```


Представляет положение нижней границы области обрезки, выраженное в виде отношения к высоте изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBottomCropInch(double value) {#setBottomCropInch-double-}
```
public void setBottomCropInch(double value)
```


Представляет положение нижней границы области обрезки, выраженное в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBrightness(double value) {#setBrightness-double-}
```
public void setBrightness(double value)
```


Представляет изменение яркости изображения в процентах.

**Remarks**

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setContrast(double value) {#setContrast-double-}
```
public void setContrast(double value)
```


Представляет изменение контрастности изображения в процентах.

**Remarks**

Значение находится в диапазоне от -100% до 100%. Работает так же, как в Excel 2007 и более новых версиях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setGamma(double value) {#setGamma-double-}
```
public void setGamma(double value)
```


Представляет гамму изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setGray(boolean value) {#setGray-boolean-}
```
public void setGray(boolean value)
```


Указывает, должно ли это изображение отображаться в градациях серого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLeftCrop(double value) {#setLeftCrop-double-}
```
public void setLeftCrop(double value)
```


Представляет положение левой границы области обрезки, выраженное в виде отношения к ширине изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLeftCropInch(double value) {#setLeftCropInch-double-}
```
public void setLeftCropInch(double value)
```


Представляет положение левой границы области обрезки, выраженное в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRightCrop(double value) {#setRightCrop-double-}
```
public void setRightCrop(double value)
```


Представляет положение правой границы области обрезки, выраженное в виде отношения к ширине изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRightCropInch(double value) {#setRightCropInch-double-}
```
public void setRightCropInch(double value)
```


Представляет положение правой границы области обрезки, выраженное в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopCrop(double value) {#setTopCrop-double-}
```
public void setTopCrop(double value)
```


Представляет положение верхней границы области обрезки, выраженное в виде отношения к высоте изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopCropInch(double value) {#setTopCropInch-double-}
```
public void setTopCropInch(double value)
```


Представляет положение верхней границы области обрезки, выраженное в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTransparentColor(CellsColor value) {#setTransparentColor-com.aspose.cells.CellsColor-}
```
public void setTransparentColor(CellsColor value)
```


Устанавливает прозрачный цвет изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

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

