---
title: "TextOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры текста."
type: docs
url: /ru/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Представляет параметры текста.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Проверяет, равны ли два шрифта. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Получает цвет в виде 32-битного значения ARGB. |
| [getCapsType()](#getCapsType--) | Получает тип заглавных букв для текста фигуры. |
| [getCharset()](#getCharset--) | Представляет набор символов. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Получает [Color](../../com.aspose.cells/color) шрифта. |
| [getDoubleSize()](#getDoubleSize--) | Получает двойной размер шрифта. |
| [getFarEastName()](#getFarEastName--) | Получает название FarEast. |
| [getFill()](#getFill--) | Представляет формат заливки текста. |
| [getKerning()](#getKerning--) | Указывает минимальный размер шрифта, при котором будет применяться кернинг символов для этого фрагмента текста. |
| [getLanguageCode()](#getLanguageCode--) | Получает язык пользовательского интерфейса. |
| [getLatinName()](#getLatinName--) | Получает латинское название. |
| [getName()](#getName--) | Получает имя фигуры. |
| [getOutline()](#getOutline--) | Представляет формат контура текста. |
| [getSchemeType()](#getSchemeType--) | Получает тип схемы шрифта. |
| [getScriptOffset()](#getScriptOffset--) | Получает смещение скрипта, в процентах |
| [getShadow()](#getShadow--) | Представляет объект [ShadowEffect](../../com.aspose.cells/shadoweffect), определяющий эффект тени для элемента диаграммы или фигуры. |
| [getSize()](#getSize--) | Получает размер шрифта. |
| [getSpacing()](#getSpacing--) | Указывает интервал между символами в текстовом фрагменте. |
| [getStrikeType()](#getStrikeType--) | Получает тип перечёркивания текста. |
| [getThemeColor()](#getThemeColor--) | Получает цвет темы. |
| [getUnderline()](#getUnderline--) | Получает тип подчеркивания шрифта. |
| [getUnderlineColor()](#getUnderlineColor--) | Получает цвет подчеркивания. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Получает значение, указывающее, является ли шрифт полужирным. |
| [isItalic()](#isItalic--) | Получает значение, указывающее, является ли шрифт курсивом. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Указывает, следует ли применять нормализацию высоты к текстовому фрагменту. |
| [isStrikeout()](#isStrikeout--) | Получает значение, указывающее, имеет ли шрифт одиночное перечёркивание. |
| [isSubscript()](#isSubscript--) | Получает значение, указывающее, является ли шрифт нижним индексом. |
| [isSuperscript()](#isSuperscript--) | Получает значение, указывающее, является ли шрифт верхним индексом. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Устанавливает цвет в виде 32-битного значения ARGB. |
| [setBold(boolean value)](#setBold-boolean-) | Устанавливает значение, указывающее, является ли шрифт полужирным. |
| [setCapsType(int value)](#setCapsType-int-) | Устанавливает тип заглавных букв для текста формы. |
| [setCharset(int value)](#setCharset-int-) | Представляет набор символов. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Устанавливает [Color](../../com.aspose.cells/color) шрифта. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Устанавливает двойной размер шрифта. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Устанавливает название FarEast. |
| [setItalic(boolean value)](#setItalic-boolean-) | Устанавливает значение, указывающее, является ли шрифт курсивом. |
| [setKerning(double value)](#setKerning-double-) | Указывает минимальный размер шрифта, при котором будет применяться кернинг символов для этого фрагмента текста. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Устанавливает язык пользовательского интерфейса. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Устанавливает латинское название. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя объекта. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Устанавливает имя и схему шрифта. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Указывает, следует ли применять нормализацию высоты к текстовому фрагменту. |
| [setSchemeType(int value)](#setSchemeType-int-) | Устанавливает тип схемы шрифта. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Устанавливает смещение скрипта, в процентах |
| [setSize(int value)](#setSize-int-) | Устанавливает размер шрифта. |
| [setSpacing(double value)](#setSpacing-double-) | Указывает интервал между символами в текстовом фрагменте. |
| [setStrikeType(int value)](#setStrikeType-int-) | Получает тип перечёркивания текста. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Устанавливает значение, указывающее, зачеркивается ли шрифт одинарно. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Устанавливает значение, указывающее, является ли шрифт нижним индексом. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Устанавливает значение, указывающее, является ли шрифт верхним индексом. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет темы. |
| [setUnderline(int value)](#setUnderline-int-) | Устанавливает тип подчеркивания шрифта. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Устанавливает цвет подчеркивания. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Cell. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Проверяет, равны ли два шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Сравненный объект шрифта. |

**Returns:**
boolean — True, если равен сравниваемому объекту шрифта.
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Получает цвет в виде 32-битного значения ARGB.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Получает тип заглавных букв для текста фигуры.

Смотрите [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Представляет набор символов.

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


Получает [Color](../../com.aspose.cells/color) шрифта.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Получает двойной размер шрифта.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Получает название FarEast.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Представляет формат заливки текста.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Указывает минимальный размер шрифта, при котором будет применяться кернинг символов для этого фрагмента текста.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Получает язык пользовательского интерфейса.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Получает латинское название.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Получает имя фигуры.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Представляет формат контура текста.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Получает тип схемы шрифта.

Смотрите [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Получает смещение скрипта, в процентах

**Remarks**

Только для фигур и диаграмм.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Представляет объект [ShadowEffect](../../com.aspose.cells/shadoweffect), определяющий эффект тени для элемента диаграммы или фигуры.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Получает размер шрифта.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Указывает интервал между символами в текстовом фрагменте.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Получает тип перечёркивания текста.

Смотрите [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Получает цвет темы.

**Remarks**

Если цвет шрифта не является цветом темы, будет возвращено NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Получает тип подчеркивания шрифта.

Смотрите [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Получает цвет подчеркивания.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Получает значение, указывающее, является ли шрифт полужирным.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Получает значение, указывающее, является ли шрифт курсивом.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Указывает, следует ли применять нормализацию высоты к текстовому фрагменту.

**Remarks**

Только для шрифтов фигур или диаграмм.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Получает значение, указывающее, имеет ли шрифт одиночное перечёркивание.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Получает значение, указывающее, является ли шрифт нижним индексом.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Получает значение, указывающее, является ли шрифт верхним индексом.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Устанавливает цвет в виде 32-битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Устанавливает значение, указывающее, является ли шрифт полужирным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Устанавливает тип заглавных букв для текста формы.

Смотрите [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Представляет набор символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Устанавливает [Color](../../com.aspose.cells/color) шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Устанавливает двойной размер шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Устанавливает название FarEast.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Устанавливает значение, указывающее, является ли шрифт курсивом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Указывает минимальный размер шрифта, при котором будет применяться кернинг символов для этого фрагмента текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Устанавливает язык пользовательского интерфейса.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Устанавливает латинское название.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Устанавливает имя и схему шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Указывает, следует ли применять нормализацию высоты к текстовому фрагменту.

**Remarks**

Только для шрифтов фигур или диаграмм.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Устанавливает тип схемы шрифта.

Смотрите [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Устанавливает смещение скрипта, в процентах

**Remarks**

Только для фигур и диаграмм.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Устанавливает размер шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Указывает интервал между символами в текстовом фрагменте.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Получает тип перечёркивания текста.

Смотрите [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Устанавливает значение, указывающее, зачеркивается ли шрифт одинарно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Устанавливает значение, указывающее, является ли шрифт нижним индексом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Устанавливает значение, указывающее, является ли шрифт верхним индексом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Устанавливает цвет темы.

**Remarks**

Если цвет шрифта не является цветом темы, будет возвращено NULL.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Устанавливает тип подчеркивания шрифта.

Смотрите [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Устанавливает цвет подчеркивания.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект Cell.

**Returns:**
java.lang.String -
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

