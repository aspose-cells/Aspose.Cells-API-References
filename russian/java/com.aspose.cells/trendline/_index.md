---
title: "Trendline"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет линию тренда в диаграмме."
type: docs
url: /ru/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Представляет линию тренда в диаграмме.

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
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется назад. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Указывает длину наконечника стрелки для начала линии. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Указывает ширину наконечника стрелки для начала линии. |
| [getBeginType()](#getBeginType--) | Указывает наконечник стрелки для начала линии. |
| [getCapType()](#getCapType--) | Указывает конечные заглушки. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Представляет [Color](../../com.aspose.cells/color) линии. |
| [getCompoundType()](#getCompoundType--) | Указывает составной тип линии |
| [getDashType()](#getDashType--) | Указывает тип пунктирной линии |
| [getDataLabels()](#getDataLabels--) | Представляет объект DataLabels для указанной серии. |
| [getDisplayEquation()](#getDisplayEquation--) | Указывает, отображается ли уравнение трендлинии на диаграмме (в той же подписи данных, что и значение R‑квадрат). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Указывает, отображается ли значение R‑квадрат трендлинии на диаграмме (в той же подписи данных, что и уравнение). |
| [getEndArrowLength()](#getEndArrowLength--) | Указывает длину наконечника стрелки для конца линии. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Указывает ширину наконечника стрелки для конца линии. |
| [getEndType()](#getEndType--) | Указывает тип наконечника стрелки для конца линии. |
| [getFormattingType()](#getFormattingType--) | Получает тип формата. |
| [getForward()](#getForward--) | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендлиния продолжается вперёд. |
| [getGradientFill()](#getGradientFill--) | Представляет градиентную заливку. |
| [getIntercept()](#getIntercept--) | Возвращает или задает точку, где трендлиния пересекает ось значений. |
| [getJoinType()](#getJoinType--) | Указывает соединительные заглушки. |
| [getLegendEntry()](#getLegendEntry--) | Получает запись легенды, соответствующую этой трендлинии. |
| [getName()](#getName--) | Возвращает имя трендлинии. |
| [getOrder()](#getOrder--) | Возвращает или задает порядок трендлинии (целое число больше 1), когда тип трендлинии — Полиномиальный. |
| [getPeriod()](#getPeriod--) | Возвращает или задает период для скользящей средней трендлинии. |
| [getStyle()](#getStyle--) | Представляет стиль линии. |
| [getThemeColor()](#getThemeColor--) | Получает цвет темы. |
| [getTransparency()](#getTransparency--) | Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [getType()](#getType--) | Возвращает тип трендлинии. |
| [getWeight()](#getWeight--) | Получает [WeightType](../../com.aspose.cells/weighttype) линии. |
| [getWeightPt()](#getWeightPt--) | Получает толщину линии в единицах пунктов. |
| [getWeightPx()](#getWeightPx--) | Получает толщину линии в пикселях. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Указывает, автоматически ли назначен этот стиль линии. |
| [isAutomaticColor()](#isAutomaticColor--) | Указывает, автоматически ли назначен цвет линии. |
| [isInterceptAuto()](#isInterceptAuto--) | Указывает, автоматически ли Microsoft Workbook определяет точку пересечения трендовой линии. |
| [isNameAuto()](#isNameAuto--) | Возвращает, автоматически ли Microsoft Excel определяет название трендовой линии. |
| [isVisible()](#isVisible--) | Отображает, видима ли линия. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Указывает, автоматически ли назначен этот стиль линии. |
| [setBackward(double value)](#setBackward-double-) | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется назад. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Указывает длину наконечника стрелки для начала линии. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Указывает ширину наконечника стрелки для начала линии. |
| [setBeginType(int value)](#setBeginType-int-) | Указывает наконечник стрелки для начала линии. |
| [setCapType(int value)](#setCapType-int-) | Указывает конечные заглушки. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Представляет [Color](../../com.aspose.cells/color) линии. |
| [setCompoundType(int value)](#setCompoundType-int-) | Указывает составной тип линии |
| [setDashType(int value)](#setDashType-int-) | Указывает тип пунктирной линии |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Указывает, отображается ли уравнение трендлинии на диаграмме (в той же подписи данных, что и значение R‑квадрат). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Указывает, отображается ли значение R‑квадрат трендлинии на диаграмме (в той же подписи данных, что и уравнение). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Указывает длину наконечника стрелки для конца линии. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Указывает ширину наконечника стрелки для конца линии. |
| [setEndType(int value)](#setEndType-int-) | Указывает тип наконечника стрелки для конца линии. |
| [setFormattingType(int value)](#setFormattingType-int-) | Устанавливает тип формата. |
| [setForward(double value)](#setForward-double-) | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендлиния продолжается вперёд. |
| [setIntercept(double value)](#setIntercept-double-) | Возвращает или задает точку, где трендлиния пересекает ось значений. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Устанавливает, автоматически ли Microsoft Workbook определяет точку пересечения трендовой линии. |
| [setJoinType(int value)](#setJoinType-int-) | Указывает соединительные заглушки. |
| [setName(String value)](#setName-java.lang.String-) | Возвращает имя трендлинии. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Возвращает, автоматически ли Microsoft Excel определяет название трендовой линии. |
| [setOrder(int value)](#setOrder-int-) | Возвращает или задает порядок трендлинии (целое число больше 1), когда тип трендлинии — Полиномиальный. |
| [setPeriod(int value)](#setPeriod-int-) | Возвращает или задает период для скользящей средней трендлинии. |
| [setStyle(int value)](#setStyle-int-) | Представляет стиль линии. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет темы. |
| [setTransparency(double value)](#setTransparency-double-) | Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [setVisible(boolean value)](#setVisible-boolean-) | Отображает, видима ли линия. |
| [setWeight(int value)](#setWeight-int-) | Устанавливает [WeightType](../../com.aspose.cells/weighttype) линии. |
| [setWeightPt(double value)](#setWeightPt-double-) | Устанавливает толщину линии в пунктах. |
| [setWeightPx(double value)](#setWeightPx-double-) | Устанавливает толщину линии в пикселях. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется назад. Количество периодов должно быть больше или равно нулю. Если тип диаграммы — столбчатая, количество периодов должно быть от 0 до 0,5.

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Указывает длину наконечника стрелки для начала линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Указывает ширину наконечника стрелки для начала линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Указывает наконечник стрелки для начала линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Указывает конечные заглушки.

См. [LineCapType](../../com.aspose.cells/linecaptype).

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


Представляет [Color](../../com.aspose.cells/color) линии.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Указывает составной тип линии

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Указывает тип пунктирной линии

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Представляет объект DataLabels для указанной серии.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Отображает, выводится ли уравнение трендовой линии на диаграмме (в той же метке данных, что и значение R‑квадрат). Установка этого свойства в True автоматически включает метки данных.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Отображает, выводится ли значение R‑квадрат трендовой линии на диаграмме (в той же метке данных, что и уравнение). Установка этого свойства в True автоматически включает метки данных.

**Returns:**
boolean
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Указывает длину наконечника стрелки для конца линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Указывает ширину наконечника стрелки для конца линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Указывает тип наконечника стрелки для конца линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Получает тип формата.

См. [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getForward() {#getForward--}
```
public double getForward()
```


Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется вперёд. Количество периодов должно быть больше или равно нулю.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Представляет градиентную заливку.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Возвращает или задает точку, где трендлиния пересекает ось значений.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Указывает соединительные заглушки.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Получает запись легенды, соответствующую этой трендлинии.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Возвращает имя трендлинии.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Возвращает или задает порядок трендовой линии (целое число больше 1), когда тип трендовой линии — Полиномиальный. Порядок должен быть от 2 до 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Возвращает или задает период для скользящей средней трендлинии.

**Remarks**

Это значение должно быть между 2 и 255. И оно должно быть меньше количества точек диаграммы в серии

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Представляет стиль линии.

Смотрите [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Получает цвет темы.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Возвращает тип трендлинии.

Смотрите [TrendlineType](../../com.aspose.cells/trendlinetype).

**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```


Получает [WeightType](../../com.aspose.cells/weighttype) линии.

Смотрите [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Получает толщину линии в единицах пунктов.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Получает толщину линии в пикселях.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


Указывает, автоматически ли назначен этот стиль линии.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Указывает, автоматически ли назначен цвет линии.

**Returns:**
boolean
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Указывает, автоматически ли Microsoft Workbook определяет точку пересечения трендовой линии.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Возвращает, автоматически ли Microsoft Excel определяет название трендовой линии.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Отображает, видима ли линия.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Указывает, автоматически ли назначен этот стиль линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется назад. Количество периодов должно быть больше или равно нулю. Если тип диаграммы — столбчатая, количество периодов должно быть от 0 до 0,5.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Указывает длину наконечника стрелки для начала линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Указывает ширину наконечника стрелки для начала линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Указывает наконечник стрелки для начала линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Представляет [Color](../../com.aspose.cells/color) линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Указывает составной тип линии

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Указывает тип пунктирной линии

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Отображает, выводится ли уравнение трендовой линии на диаграмме (в той же метке данных, что и значение R‑квадрат). Установка этого свойства в True автоматически включает метки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Отображает, выводится ли значение R‑квадрат трендовой линии на диаграмме (в той же метке данных, что и уравнение). Установка этого свойства в True автоматически включает метки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Указывает длину наконечника стрелки для конца линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Указывает ширину наконечника стрелки для конца линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Указывает тип наконечника стрелки для конца линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Устанавливает тип формата.

См. [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое трендовая линия расширяется вперёд. Количество периодов должно быть больше или равно нулю.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Возвращает или задает точку, где трендлиния пересекает ось значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Устанавливает, автоматически ли Microsoft Workbook определяет точку пересечения трендовой линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Указывает соединительные заглушки.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Возвращает имя трендлинии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Возвращает, автоматически ли Microsoft Excel определяет название трендовой линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Возвращает или задает порядок трендовой линии (целое число больше 1), когда тип трендовой линии — Полиномиальный. Порядок должен быть от 2 до 6.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Возвращает или задает период для скользящей средней трендлинии.

**Remarks**

Это значение должно быть между 2 и 255. И оно должно быть меньше количества точек диаграммы в серии

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Представляет стиль линии.

Смотрите [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Устанавливает цвет темы.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Отображает, видима ли линия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Устанавливает [WeightType](../../com.aspose.cells/weighttype) линии.

Смотрите [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Устанавливает толщину линии в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Устанавливает толщину линии в пикселях.

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

