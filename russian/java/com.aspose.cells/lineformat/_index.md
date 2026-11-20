---
title: "LineFormat"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все настройки линии."
type: docs
url: /ru/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Представляет все настройки линии.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [LineFormat](../../com.aspose.cells/lineformat). |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Получает тип длины начальной стрелки линии. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Получает тип начальной стрелки линии. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Получает тип ширины начальной стрелки линии. |
| [getCapType()](#getCapType--) | Указывает конечные заглушки. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Указывает составной тип линии. |
| [getDashStyle()](#getDashStyle--) | Указывает тип штриха линии. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Получает тип длины конечной стрелки линии. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Получает тип конечной стрелки линии. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Получает тип ширины конечной стрелки линии. |
| [getFillType()](#getFillType--) | Получает тип заполнения |
| [getGradientColor1()](#getGradientColor1--) | Возвращает градиентный цвет 1 для указанного заполнения. |
| [getGradientColor2()](#getGradientColor2--) | Возвращает градиентный цвет 2 для указанного заполнения. |
| [getGradientColorType()](#getGradientColorType--) | Возвращает тип градиентного цвета для указанного заполнения. |
| [getGradientDegree()](#getGradientDegree--) | Возвращает степень градиента для указанного заполнения. |
| [getGradientFill()](#getGradientFill--) | Получает объект [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Возвращает стиль градиента для указанного заполнения. |
| [getGradientVariant()](#getGradientVariant--) | Возвращает вариант градиента для указанного заполнения. |
| [getImageData()](#getImageData--) | Получает данные изображения картинки. |
| [getJoinType()](#getJoinType--) | Указывает тип соединения линии. |
| [getPattern()](#getPattern--) | Представляет шаблон отображения области. |
| [getPatternFill()](#getPatternFill--) | Получает объект [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--). |
| [getPictureFormatType()](#getPictureFormatType--) | Получает тип формата изображения. |
| [getPresetColor()](#getPresetColor--) | Возвращает предустановленный градиентный цвет для указанного заполнения. |
| [getScale()](#getScale--) | Получает масштаб формата изображения. |
| [getSetType()](#getSetType--) | Получает тип набора формата заполнения. |
| [getSolidFill()](#getSolidFill--) | Получает объект [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--). |
| [getTexture()](#getTexture--) | Представляет тип текстуры для указанного заполнения. |
| [getTextureFill()](#getTextureFill--) | Получает объект [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--). |
| [getTransparency()](#getTransparency--) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [getType()](#getType--) | Получает тип заполнения. |
| [getWeight()](#getWeight--) | Получает толщину линии в единицах пунктов. |
| [hashCode()](#hashCode--) | Получает хеш-код. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Устанавливает тип длины начальной стрелки линии. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Устанавливает тип начальной стрелки линии. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Устанавливает тип ширины начальной стрелки линии. |
| [setCapType(int value)](#setCapType-int-) | Указывает конечные заглушки. |
| [setCompoundType(int value)](#setCompoundType-int-) | Указывает составной тип линии. |
| [setDashStyle(int value)](#setDashStyle-int-) | Указывает тип штриха линии. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Устанавливает тип длины конечной стрелки линии. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Устанавливает тип конечной стрелки линии. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Устанавливает тип ширины конечной стрелки линии. |
| [setFillType(int value)](#setFillType-int-) | Устанавливает тип заполнения |
| [setImageData(byte[] value)](#setImageData-byte---) | Устанавливает данные изображения картинки. |
| [setJoinType(int value)](#setJoinType-int-) | Указывает тип соединения линии. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Устанавливает указанную заливку в градиент из одного цвета. |
| [setPattern(int value)](#setPattern-int-) | Представляет шаблон отображения области. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Устанавливает тип формата изображения. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Устанавливает указанное заполнение в градиент предустановленного цвета. |
| [setScale(double value)](#setScale-double-) | Устанавливает масштаб формата изображения. |
| [setSetType(int value)](#setSetType-int-) | Получает тип набора формата заполнения. |
| [setTexture(int value)](#setTexture-int-) | Представляет тип текстуры для указанного заполнения. |
| [setTransparency(double value)](#setTransparency-double-) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Устанавливает указанную заливку в двухцветный градиент. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Устанавливает указанную заливку в двухцветный градиент. |
| [setType(int value)](#setType-int-) | Устанавливает тип заливки. |
| [setWeight(double value)](#setWeight-double-) | Устанавливает толщину линии в пунктах. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [LineFormat](../../com.aspose.cells/lineformat).

**Example**

```
         //You have to make sure that the index value in this line of code exists
         LineFormat obj = workbook.getWorksheets().get(0).getShapes().get(0).getLine();
         if (lineFmt.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект [LineFormat](../../com.aspose.cells/lineformat) для сравнения с этим экземпляром. |

**Returns:**
boolean — true, если значение параметра obj совпадает со значением этого экземпляра; иначе — false. Если obj равен null, этот метод возвращает false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Получает тип длины начальной стрелки линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```


Получает тип начальной стрелки линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```


Получает тип ширины начальной стрелки линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setBeginArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Указывает конечные заглушки.

См. [LineCapType](../../com.aspose.cells/linecaptype).

**Example**

```
         lineFmt.setCapType(LineCapType.FLAT);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Указывает составной тип линии.

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Example**

```
         lineFmt.setCompoundType(MsoLineStyle.SINGLE);
```

**Returns:**
int
### getDashStyle() {#getDashStyle--}
```
public int getDashStyle()
```


Указывает тип штриха линии.

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Example**

```
         lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```

**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```


Получает тип длины конечной стрелки линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```


Получает тип конечной стрелки линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```


Получает тип ширины конечной стрелки линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Получает тип заполнения

Смотрите [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Возвращает градиентный цвет 1 для указанного заполнения.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Возвращает градиентный цвет 2 для указанного заполнения.

**Remarks**

Только когда тип цвета градиента равен GradientColorType.TwoColors, это свойство имеет смысл.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Возвращает тип градиентного цвета для указанного заполнения.

Смотрите [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Возвращает степень градиента для указанной заливки. Применяется только для Excel 2007.

**Remarks**

Может принимать только значение от 0.0 (темный) до 1.0 (светлый).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Получает объект [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--).

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Возвращает стиль градиента для указанного заполнения.

См. [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Возвращает вариант градиента для указанной заливки. Применяется только для Excel 2007.

**Remarks**

Может принимать только значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль — GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Получает данные изображения картинки.

**Remarks**

Если формат заливки не является пользовательским форматом текстуры, возвращает null.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Указывает тип соединения линии.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Example**

```
         lineFmt.setJoinType(LineJoinType.ROUND);
```

**Returns:**
int
### getPattern() {#getPattern--}
```
public int getPattern()
```


Представляет шаблон отображения области.

Смотрите [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Получает объект [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--).

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Получает тип формата изображения.

Смотрите [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Возвращает предустановленный градиентный цвет для указанного заполнения.

Смотрите [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Получает масштаб формата изображения.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Получает тип набора формата заполнения.

Смотрите [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Получает объект [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--).

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Представляет тип текстуры для указанного заполнения.

См. [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Получает объект [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--).

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Получает тип заполнения.

Смотрите [FillType](../../com.aspose.cells/filltype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Получает толщину линии в единицах пунктов.

**Example**

```
         lineFmt.setWeight(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Получает хеш-код.

**Example**

```
         int hashCode = lineFmt.hashCode();
```

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




### setBeginArrowheadLength(int value) {#setBeginArrowheadLength-int-}
```
public void setBeginArrowheadLength(int value)
```


Устанавливает тип длины начальной стрелки линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Устанавливает тип начальной стрелки линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Устанавливает тип ширины начальной стрелки линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Указывает конечные заглушки.

См. [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Указывает составной тип линии.

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Указывает тип штриха линии.

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Устанавливает тип длины конечной стрелки линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Устанавливает тип конечной стрелки линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Устанавливает тип ширины конечной стрелки линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Устанавливает тип заполнения

Смотрите [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Устанавливает данные изображения картинки.

**Remarks**

Если формат заливки не является пользовательским форматом текстуры, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Указывает тип соединения линии.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Представляет шаблон отображения области.

Смотрите [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Устанавливает тип формата изображения.

Смотрите [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Устанавливает указанную заливку в градиент предустановленного цвета. Применяется только для Excel 2007.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Тип предустановленного цвета |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Стиль затенения градиента. |
| вариант | int | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Устанавливает масштаб формата изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Получает тип набора формата заполнения.

Смотрите [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Представляет тип текстуры для указанного заполнения.

См. [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип заливки.

Смотрите [FillType](../../com.aspose.cells/filltype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FillFormat.FillType. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Устанавливает толщину линии в пунктах.

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

