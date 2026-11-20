---
title: "TextParagraph"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройку абзаца текста."
type: docs
url: /ru/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Представляет настройку абзаца текста.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Получает тип горизонтального выравнивания текста абзаца. |
| [getBullet()](#getBullet--) | Получает маркер. |
| [getChildren()](#getChildren--) | Получает все текстовые фрагменты в этом абзаце. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Получает размер по умолчанию для символа табуляции в этом абзаце. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Указывает размер отступа, который будет применён к первой строке текста в абзаце. |
| [getFont()](#getFont--) | Возвращает шрифт этого объекта. |
| [getFontAlignType()](#getFontAlignType--) | Определяет, где вертикально на строке текста располагаются фактические слова. |
| [getLeftMargin()](#getLeftMargin--) | Указывает левый отступ абзаца. |
| [getLength()](#getLength--) | Получает длину символов. |
| [getLineSpace()](#getLineSpace--) | Получает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Получает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [getRightMargin()](#getRightMargin--) | Указывает правый отступ абзаца. |
| [getSpaceAfter()](#getSpaceAfter--) | Получает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Получает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [getSpaceBefore()](#getSpaceBefore--) | Получает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Получает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [getStartIndex()](#getStartIndex--) | Получает начальный индекс символов. |
| [getStops()](#getStops--) | Получает список табуляций. |
| [getTextOptions()](#getTextOptions--) | Возвращает параметры текста. |
| [getType()](#getType--) | Получает тип текстового узла. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Указывает, может ли слово восточно-азиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Устанавливает тип горизонтального выравнивания текста абзаца. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Устанавливает размер по умолчанию для символа табуляции в этом абзаце. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Указывает, может ли слово восточно-азиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Указывает размер отступа, который будет применён к первой строке текста в абзаце. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Определяет, где вертикально на строке текста располагаются фактические слова. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Указывает левый отступ абзаца. |
| [setLineSpace(double value)](#setLineSpace-double-) | Устанавливает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Устанавливает количество вертикального пробела, которое будет использоваться внутри абзаца. |
| [setRightMargin(double value)](#setRightMargin-double-) | Указывает правый отступ абзаца. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Устанавливает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Устанавливает количество вертикального пробела, которое будет присутствовать после абзаца. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Устанавливает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Устанавливает количество вертикального пробела, которое будет присутствовать перед абзацем. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Устанавливает предустановленный стиль WordArt. |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Получает тип горизонтального выравнивания текста абзаца.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Получает маркер.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Получает все текстовые фрагменты в этом абзаце. Если абзац пуст, возвращает сам абзац.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Получает размер по умолчанию для символа табуляции в этом абзаце.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Указывает размер отступа, который будет применён к первой строке текста в абзаце.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Возвращает шрифт этого объекта.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Определяет, где вертикально на строке текста располагаются фактические слова. Это относится к вертикальному размещению символов относительно базовых линий.

См. [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Указывает левый отступ абзаца.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Получает длину символов.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Получает количество вертикального пробела, которое будет использоваться внутри абзаца.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Получает количество вертикального пробела, которое будет использоваться внутри абзаца.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Указывает правый отступ абзаца.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Получает количество вертикального пробела, которое будет присутствовать после абзаца.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Получает количество вертикального пробела, которое будет присутствовать после абзаца.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Получает количество вертикального пробела, которое будет присутствовать перед абзацем.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Получает количество вертикального пробела, которое будет присутствовать перед абзацем.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Получает начальный индекс символов.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Получает список табуляций.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Возвращает параметры текста.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Получает тип текстового узла.

Смотрите [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Указывает, может ли слово восточно-азиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Устанавливает тип горизонтального выравнивания текста абзаца.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Устанавливает размер по умолчанию для символа табуляции в этом абзаце.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Указывает, может ли слово восточно-азиатского языка быть разбито пополам и перенесено на следующую строку без добавления дефиса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Указывает размер отступа, который будет применён к первой строке текста в абзаце.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Определяет, где вертикально на строке текста располагаются фактические слова. Это относится к вертикальному размещению символов относительно базовых линий.

См. [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Указывает, должна ли пунктуация принудительно размещаться в строке текста или переноситься на другую строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Указывает, может ли латинское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Указывает левый отступ абзаца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Устанавливает количество вертикального пробела, которое будет использоваться внутри абзаца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Устанавливает количество вертикального пробела, которое будет использоваться внутри абзаца.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Указывает правый отступ абзаца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Устанавливает количество вертикального пробела, которое будет присутствовать после абзаца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Устанавливает количество вертикального пробела, которое будет присутствовать после абзаца.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Устанавливает количество вертикального пробела, которое будет присутствовать перед абзацем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Устанавливает количество вертикального пробела, которое будет присутствовать перед абзацем.

См. [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Устанавливает предустановленный стиль WordArt.

**Remarks**

Только для текста фигуры/диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Предустановленный стиль WordArt. |

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

