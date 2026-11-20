---
title: "FillFormat"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий формат заливки фигуры."
type: docs
url: /ru/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

Инкапсулирует объект, представляющий формат заливки фигуры.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Filling the area of the 2nd NSeries with a gradient
         chart.getNSeries().get(seriesIndex).getArea().getFillFormat().setOneColorGradient(Color.getLime(), 1, GradientStyleType.HORIZONTAL, 1);
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Получает тип заполнения |
| [getGradientColor1()](#getGradientColor1--) | Возвращает градиентный цвет 1 для указанного заполнения. |
| [getGradientColor2()](#getGradientColor2--) | Возвращает градиентный цвет 2 для указанного заполнения. |
| [getGradientColorType()](#getGradientColorType--) | Возвращает тип градиентного цвета для указанного заполнения. |
| [getGradientDegree()](#getGradientDegree--) | Возвращает степень градиента для указанного заполнения. |
| [getGradientFill()](#getGradientFill--) | Получает объект [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Возвращает стиль градиента для указанного заполнения. |
| [getGradientVariant()](#getGradientVariant--) | Возвращает вариант градиента для указанного заполнения. |
| [getImageData()](#getImageData--) | Получает данные изображения картинки. |
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
| [hashCode()](#hashCode--) | Получает хеш-код. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Устанавливает тип заполнения |
| [setImageData(byte[] value)](#setImageData-byte---) | Устанавливает данные изображения картинки. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

