---
title: "GradientFill"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет градиентную заливку."
type: docs
url: /ru/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Представляет градиентную заливку.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | Угол линейного заполнения. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Получает тип направления градиента. |
| [getFillType()](#getFillType--) | Получает тип заполнения градиентом. |
| [getGradientColor1()](#getGradientColor1--) | Получает градиентный цвет 1. |
| [getGradientColor2()](#getGradientColor2--) | Получает градиентный цвет 2. |
| [getGradientColorType()](#getGradientColorType--) | Получает тип градиентного цвета. |
| [getGradientDegree()](#getGradientDegree--) | Получает степень градиента. |
| [getGradientStops()](#getGradientStops--) | Представляет коллекцию градиентных остановок. |
| [getGradientStyle()](#getGradientStyle--) | Получает тип стиля градиента. |
| [getPresetColor()](#getPresetColor--) | Возвращает предустановленный градиентный цвет для указанного заполнения. |
| [getVariant()](#getVariant--) | Получает вариант. |
| [hashCode()](#hashCode--) | Получает хеш-код. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | Угол линейного заполнения. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Установите тип заливки градиентом и направление. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Устанавливает указанную заливку в градиент из одного цвета. |
| [setPresetColor(int value)](#setPresetColor-int-) | Возвращает предустановленный градиентный цвет для указанного заполнения. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Устанавливает указанное заполнение в градиент предустановленного цвета. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Устанавливает предустановленную тематическую заливку градиентом. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Устанавливает указанную заливку в двухцветный градиент. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Устанавливает указанную заливку в двухцветный градиент. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


/

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


Угол линейного заполнения.

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Получает тип направления градиента.

Смотрите [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Получает тип заполнения градиентом.

Смотрите [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Получает градиентный цвет 1. Применяется к Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Получает градиентный цвет 2. Применяется к Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Получает тип градиентного цвета. Применяется к Excel97-2003

Смотрите [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Получает степень градиента. Применяется к Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Представляет коллекцию градиентных остановок.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Получает тип стиля градиента. Применяется к Excel97-2003

См. [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Возвращает предустановленный цвет градиента для указанной заливки. Применяется к Excel97-2003

Смотрите [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Получает вариант. Применяется к Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Получает хеш-код.

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAngle(float value) {#setAngle-float-}
```
public void setAngle(float value)
```


Угол линейного заполнения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Установите тип заливки градиентом и направление.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Тип заливки градиентом. |
| угол | double | Угол. Применяется только для GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Тип направления. Применяется только для GradientFillType.Radial и GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Устанавливает указанную заливку в одноцветный градиент. Применяется только для Excel 2007.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Один цвет градиента. |
| степень | double | Степень градиента. Может принимать значение от 0.0 (темный) до 1.0 (светлый). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Возвращает предустановленный цвет градиента для указанной заливки. Применяется к Excel97-2003

Смотрите [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Устанавливает указанную заливку в градиент предустановленного цвета. Применяется только к Excel 97-2003

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Тип предустановленного цвета |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Устанавливает предустановленную тематическую заливку градиентом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Тип предустановленного градиента. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Тип цветовой темы. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Устанавливает указанную заливку в двухцветный градиент. Применяется только для Excel 2007.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Один цвет градиента. |
| color2 | [Color](../../com.aspose.cells/color) | Два цвета градиента. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Устанавливает указанную заливку в двухцветный градиент. Применяется только для Excel 2007.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Один цвет градиента. |
| transparency1 | double | Степень прозрачности цвета1 в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| color2 | [Color](../../com.aspose.cells/color) | Два цвета градиента. |
| transparency2 | double | Степень прозрачности цвета2 в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

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

