---
title: "RenderingWatermark"
second_title: "Справочник API Aspose.Cells for Java"
description: "Водяной знак для рендеринга."
type: docs
url: /ru/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Водяной знак для рендеринга.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Создает экземпляр текстового водяного знака. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Создает экземпляр графического водяного знака. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Получает шрифт водяного знака. |
| [getHAlignment()](#getHAlignment--) | Получает горизонтальное выравнивание водяного знака относительно страницы. |
| [getImage()](#getImage--) | Получает изображение водяного знака. |
| [getOffsetX()](#getOffsetX--) | Получает значение смещения к [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Получает значение смещения к [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Получает непрозрачность водяного знака в диапазоне [0, 1]. |
| [getRotation()](#getRotation--) | Получает вращение водяного знака в градусах. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Получает масштаб относительно целевой страницы в процентах. |
| [getText()](#getText--) | Получает текст водяного знака. |
| [getVAlignment()](#getVAlignment--) | Получает вертикальное выравнивание водяного знака относительно страницы. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Указывает, размещен ли водяной знак за содержимым страницы. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Указывает, размещен ли водяной знак за содержимым страницы. |
| [setHAlignment(int value)](#setHAlignment-int-) | Устанавливает горизонтальное выравнивание водяного знака относительно страницы. |
| [setOffsetX(float value)](#setOffsetX-float-) | Устанавливает значение смещения к [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Устанавливает значение смещения к [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Устанавливает непрозрачность водяного знака в диапазоне [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Устанавливает вращение водяного знака в градусах. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Устанавливает масштаб относительно целевой страницы в процентах. |
| [setVAlignment(int value)](#setVAlignment-int-) | Устанавливает вертикальное выравнивание водяного знака относительно страницы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Создает экземпляр текстового водяного знака.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | текст водяного знака |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | шрифт водяного знака |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Создает экземпляр графического водяного знака.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Получает шрифт водяного знака.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Получает горизонтальное выравнивание водяного знака относительно страницы.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Допустимы только Left, Center, Right. По умолчанию Left.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Получает изображение водяного знака.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Получает значение смещения к [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Получает значение смещения к [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Получает непрозрачность водяного знака в диапазоне [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Получает вращение водяного знака в градусах.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Получает масштаб относительно целевой страницы в процентах.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Получает текст водяного знака.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Получает вертикальное выравнивание водяного знака относительно страницы.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Допустимы только Top, Center, Bottom. По умолчанию Top.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


Указывает, размещен ли водяной знак за содержимым страницы.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


Указывает, размещен ли водяной знак за содержимым страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Устанавливает горизонтальное выравнивание водяного знака относительно страницы.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Допустимы только Left, Center, Right. По умолчанию Left.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Устанавливает значение смещения к [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Устанавливает значение смещения к [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Устанавливает непрозрачность водяного знака в диапазоне [0, 1].

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Устанавливает вращение водяного знака в градусах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Устанавливает масштаб относительно целевой страницы в процентах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Устанавливает вертикальное выравнивание водяного знака относительно страницы.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Допустимы только Top, Center, Bottom. По умолчанию Top.

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

