---
title: "TextEffectFormat"
second_title: "Справочник API Aspose.Cells for Java"
description: "Содержит свойства и методы, применимые к объектам WordArt."
type: docs
url: /ru/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Содержит свойства и методы, применимые к объектам WordArt.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
         TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
         textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
         workbook.save("Book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Указывает, является ли шрифт полужирным. |
| [getFontItalic()](#getFontItalic--) | Указывает, является ли шрифт курсивом. |
| [getFontName()](#getFontName--) | Имя шрифта, используемого в WordArt. |
| [getFontSize()](#getFontSize--) | Размер (в пунктах) шрифта, используемого в WordArt. |
| [getPresetShape()](#getPresetShape--) | Получает тип предустановленной фигуры. |
| [getRotatedChars()](#getRotatedChars--) | Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt. |
| [getText()](#getText--) | Текст в WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Указывает, является ли шрифт полужирным. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Указывает, является ли шрифт курсивом. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Имя шрифта, используемого в WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | Размер (в пунктах) шрифта, используемого в WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Устанавливает тип предустановленной фигуры. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt. |
| [setText(String value)](#setText-java.lang.String-) | Текст в WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Устанавливает предустановленный текстовый эффект. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```


Указывает, является ли шрифт полужирным.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Указывает, является ли шрифт курсивом.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


Имя шрифта, используемого в WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Размер (в пунктах) шрифта, используемого в WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Получает тип предустановленной фигуры.

См. [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Текст в WordArt.

**Returns:**
java.lang.String
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




### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```


Указывает, является ли шрифт полужирным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Указывает, является ли шрифт курсивом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Имя шрифта, используемого в WordArt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Размер (в пунктах) шрифта, используемого в WordArt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Устанавливает тип предустановленной фигуры.

См. [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Текст в WordArt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Устанавливает предустановленный текстовый эффект.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Предустановленный текстовый эффект. |

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

