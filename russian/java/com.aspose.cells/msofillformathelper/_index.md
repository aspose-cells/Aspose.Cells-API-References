---
title: "MsoFillFormatHelper"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет формат заполнения для фигуры."
type: docs
url: /ru/java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

Представляет формат заполнения для фигуры.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Получает цвет фона файла. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Получает основной цвет заливки. |
| [getForeColorTransparency()](#getForeColorTransparency--) | Возвращает или задает степень переднего цвета указанной заливки в диапазоне от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [getImageData()](#getImageData--) | Получает данные текстурной и изображенческой заливки. |
| [getTexture()](#getTexture--) | Получает тип текстурной заливки. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Указывает, есть ли заливка. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Устанавливает цвет фона файла. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Устанавливает основной цвет заливки. |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | Возвращает или задает степень переднего цвета указанной заливки в диапазоне от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [setImageData(byte[] value)](#setImageData-byte---) | Устанавливает данные текстурной и изображенческой заливки. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Устанавливает указанную заливку в градиент из одного цвета. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, есть ли заливка. |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Получает цвет фона файла.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Получает основной цвет заливки.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


Возвращает или задает степень переднего цвета указанной заливки в диапазоне от 0.0 (непрозрачный) до 1.0 (прозрачный).

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Получает данные текстурной и изображенческой заливки.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Получает тип текстурной заливки.

См. [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, есть ли заливка.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


Устанавливает цвет фона файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Устанавливает основной цвет заливки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


Возвращает или задает степень переднего цвета указанной заливки в диапазоне от 0.0 (непрозрачный) до 1.0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Устанавливает данные текстурной и изображенческой заливки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Устанавливает указанную заливку в градиент из одного цвета.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Один цвет градиента. |
| степень | double | Степень градиента. Может принимать значение от 0.0 (темный) до 1.0 (светлый). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, есть ли заливка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

