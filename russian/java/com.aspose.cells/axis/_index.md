---
title: "Axis"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий ось диаграммы."
type: docs
url: /ru/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Инкапсулирует объект, представляющий ось диаграммы.

**Example**

Из приведённого кода вы можете узнать, как установить единицу измерения, максимальное и минимальное значение оси.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Получает [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Определяет, пересекает ли ось значений ось категорий между категориями. |
| [getAxisLabels()](#getAxisLabels--) | Получает метки оси после вызова метода Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | Получает внешний вид оси. |
| [getAxisTexts()](#getAxisTexts--) | Получает метки оси после вызова метода Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | Представляет масштаб базовой единицы для оси категорий. |
| [getBins()](#getBins--) | Представляет интервалы на оси диаграммы (гистограмма/парето) |
| [getCategoryType()](#getCategoryType--) | Представляет тип оси категорий. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Представляет точку на оси значений, где ось категорий её пересекает. |
| [getCrossType()](#getCrossType--) | Представляет [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) на указанной оси, где пересекается другая ось. |
| [getCustUnit()](#getCustUnit--) | Указывает пользовательское значение для единицы отображения. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Указывает пользовательское значение для единицы отображения. |
| [getCustomUnit()](#getCustomUnit--) | Указывает пользовательское значение для единицы отображения. |
| [getDisplayUnit()](#getDisplayUnit--) | Представляет подпись единицы для указанной оси. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Представляет подпись единицы на оси в указанной диаграмме. |
| [getLogBase()](#getLogBase--) | Представляет логарифмическую основу. |
| [getMajorGridLines()](#getMajorGridLines--) | Представляет основные линии сетки на оси диаграммы. |
| [getMajorTickMark()](#getMajorTickMark--) | Представляет тип основной метки деления для указанной оси. |
| [getMajorUnit()](#getMajorUnit--) | Представляет основные единицы измерения для оси. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Представляет масштаб основной единицы для оси категорий. |
| [getMaxValue()](#getMaxValue--) | Представляет максимальное значение на оси значений. |
| [getMinValue()](#getMinValue--) | Представляет минимальное значение на оси значений. |
| [getMinorGridLines()](#getMinorGridLines--) | Представляет вспомогательные линии сетки на оси диаграммы. |
| [getMinorTickMark()](#getMinorTickMark--) | Представляет тип вспомогательной метки деления для указанной оси. |
| [getMinorUnit()](#getMinorUnit--) | Представляет вспомогательные единицы измерения для оси. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Представляет масштаб основной единицы для оси категорий. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Представляет положение меток делений на указанной оси. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Представляет количество категорий или рядов между метками делений. |
| [getTickLabels()](#getTickLabels--) | Возвращает объект [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) , который представляет метки делений для указанной оси. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Возвращает или задает количество категорий или рядов между метками делений. |
| [getTitle()](#getTitle--) | Получает заголовок этой оси в диаграмме. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Указывает, должны ли метки отображаться многоуровневым способом. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Указывает, является ли интервал между метками делений автоматическим. |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Указывает, назначается ли основная единица оси автоматически. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Указывает, назначается ли максимальное значение автоматически. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Указывает, назначается ли минимальное значение автоматически. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Указывает, назначается ли вспомогательная единица оси автоматически. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Представляет, является ли базовая единица автоматической. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Представляет, отображается ли метка единицы отображения на указанной оси. |
| [isLogarithmic()](#isLogarithmic--) | Представляет, является ли тип шкалы оси значений логарифмическим. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Представляет, отображает ли Microsoft Excel точки данных от последней к первой. |
| [isVisible()](#isVisible--) | Представляет, видна ли ось. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Указывает, является ли интервал между метками делений автоматическим. |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Указывает, назначается ли основная единица оси автоматически. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Указывает, назначается ли максимальное значение автоматически. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Указывает, назначается ли минимальное значение автоматически. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Указывает, назначается ли вспомогательная единица оси автоматически. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Определяет, пересекает ли ось значений ось категорий между категориями. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Представляет, является ли базовая единица автоматической. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Представляет масштаб базовой единицы для оси категорий. |
| [setCategoryType(int value)](#setCategoryType-int-) | Представляет тип оси категорий. |
| [setCrossAt(double value)](#setCrossAt-double-) | Представляет точку на оси значений, где ось категорий её пересекает. |
| [setCrossType(int value)](#setCrossType-int-) | Представляет [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) на указанной оси, где пересекается другая ось. |
| [setCustUnit(int value)](#setCustUnit-int-) | Указывает пользовательское значение для единицы отображения. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Указывает пользовательское значение для единицы отображения. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Указывает пользовательское значение для единицы отображения. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Представляет подпись единицы для указанной оси. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Представляет, отображается ли метка единицы отображения на указанной оси. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Указывает, должны ли метки отображаться многоуровневым способом. |
| [setLogBase(double value)](#setLogBase-double-) | Представляет логарифмическую основу. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Представляет, является ли тип шкалы оси значений логарифмическим. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Представляет тип основной метки деления для указанной оси. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Представляет основные единицы измерения для оси. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Представляет масштаб основной единицы для оси категорий. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Представляет максимальное значение на оси значений. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Представляет минимальное значение на оси значений. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Представляет тип вспомогательной метки деления для указанной оси. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Представляет вспомогательные единицы измерения для оси. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Представляет масштаб основной единицы для оси категорий. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Представляет, отображает ли Microsoft Excel точки данных от последней к первой. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Представляет положение меток делений на указанной оси. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Представляет количество категорий или рядов между метками делений. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Возвращает или задает количество категорий или рядов между метками делений. |
| [setVisible(boolean value)](#setVisible-boolean-) | Представляет, видна ли ось. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Получает [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Определяет, пересекает ли ось значений ось категорий между категориями.

**Remarks**

Это свойство применяется только к осям категорий и не применяется к 3‑D диаграммам.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Получает метки оси после вызова метода Chart.Calculate().

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте метод Axis.GetAxisTexts. Это свойство будет удалено через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Получает внешний вид оси.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Получает метки оси после вызова метода Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Представляет масштаб базовой единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Действует только когда свойство CategoryType установлено в TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Представляет интервалы на оси диаграммы (гистограмма/парето)

**Remarks**

Только для гистограммы или диаграммы Парето.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Представляет тип оси категорий.

Смотрите [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Представляет точку на оси значений, где ось категорий её пересекает.

**Remarks**

Число должно быть целым, когда оно применяется к категориальной оси. И значение должно быть от 1 до 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Представляет [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) на указанной оси, где пересекается другая ось.

Смотрите [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Указывает пользовательское значение для единицы отображения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство Axis.CustomUnit. Это свойство будет удалено через 12 месяцев, начиная с января 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Указывает пользовательское значение для единицы отображения.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Указывает пользовательское значение для единицы отображения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство Axis.CustomDisplayUnit. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Представляет подпись единицы для указанной оси.

Смотрите [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Представляет метку единицы измерения на оси в указанной диаграмме. Метки единиц полезны при построении диаграмм больших значений — например, в миллионах или миллиардах.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Представляет логарифмическую основу. Значение по умолчанию — 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Представляет основные линии сетки на оси диаграммы.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Представляет тип основной метки деления для указанной оси.

Смотрите [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Представляет основные единицы измерения для оси.

**Remarks**

Основные единицы должны быть больше нуля.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Представляет масштаб основной единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Представляет максимальное значение на оси значений.

**Remarks**

Тип maxValue может быть только double или DateTime.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Представляет минимальное значение на оси значений.

**Remarks**

Тип minValue может быть только double или DateTime.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Представляет вспомогательные линии сетки на оси диаграммы.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Представляет тип вспомогательной метки деления для указанной оси.

Смотрите [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Представляет вспомогательные единицы измерения для оси.

**Remarks**

Вторичные единицы должны быть больше нуля.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Представляет масштаб основной единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Представляет положение меток делений на указанной оси.

Смотрите [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Представляет количество категорий или рядов между метками делений. Применяется только к категориальным и рядовым осям.

**Remarks**

Число должно быть от 1 до 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Возвращает объект [getTickLabels()](../../com.aspose.cells/axis\\#getTickLabels--) , который представляет метки делений для указанной оси.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Возвращает или задает количество категорий или рядов между делениями. Применяется только к категориальным и рядовым осям.

**Remarks**

Число должно быть от 1 до 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Получает заголовок этой оси в диаграмме.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Указывает, должны ли метки отображаться многоуровневым способом.

**Remarks**

Допустимо только для категориальной оси.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Указывает, является ли интервал между метками делений автоматическим.

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Указывает, назначается ли основная единица оси автоматически.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Указывает, назначается ли максимальное значение автоматически.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Указывает, назначается ли минимальное значение автоматически.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Указывает, назначается ли вспомогательная единица оси автоматически.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Представляет, является ли базовая единица автоматической.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Представляет, отображается ли метка единицы отображения на указанной оси.

**Remarks**

Значение по умолчанию — True. Работает только когда [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) не равен [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Представляет, является ли тип шкалы оси значений логарифмическим.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Представляет, отображает ли Microsoft Excel точки данных от последней к первой.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Представляет, видна ли ось.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Указывает, является ли интервал между метками делений автоматическим.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Указывает, назначается ли основная единица оси автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Указывает, назначается ли максимальное значение автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Указывает, назначается ли минимальное значение автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Указывает, назначается ли вспомогательная единица оси автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Определяет, пересекает ли ось значений ось категорий между категориями.

**Remarks**

Это свойство применяется только к осям категорий и не применяется к 3‑D диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Представляет, является ли базовая единица автоматической.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Представляет масштаб базовой единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Действует только когда свойство CategoryType установлено в TimeScale.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Представляет тип оси категорий.

Смотрите [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Представляет точку на оси значений, где ось категорий её пересекает.

**Remarks**

Число должно быть целым, когда оно применяется к категориальной оси. И значение должно быть от 1 до 31999.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Представляет [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) на указанной оси, где пересекается другая ось.

Смотрите [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Указывает пользовательское значение для единицы отображения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство Axis.CustomUnit. Это свойство будет удалено через 12 месяцев, начиная с января 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Указывает пользовательское значение для единицы отображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Указывает пользовательское значение для единицы отображения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство Axis.CustomDisplayUnit. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Представляет подпись единицы для указанной оси.

Смотрите [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Представляет, отображается ли метка единицы отображения на указанной оси.

**Remarks**

Значение по умолчанию — True. Работает только когда [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) не равен [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Указывает, должны ли метки отображаться многоуровневым способом.

**Remarks**

Допустимо только для категориальной оси.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Представляет логарифмическую основу. Значение по умолчанию — 10.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Представляет, является ли тип шкалы оси значений логарифмическим.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Представляет тип основной метки деления для указанной оси.

Смотрите [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Представляет основные единицы измерения для оси.

**Remarks**

Основные единицы должны быть больше нуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Представляет масштаб основной единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Представляет максимальное значение на оси значений.

**Remarks**

Тип maxValue может быть только double или DateTime.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Представляет минимальное значение на оси значений.

**Remarks**

Тип minValue может быть только double или DateTime.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Представляет тип вспомогательной метки деления для указанной оси.

Смотрите [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Представляет вспомогательные единицы измерения для оси.

**Remarks**

Вторичные единицы должны быть больше нуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Представляет масштаб основной единицы для оси категорий.

Смотрите [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Представляет, отображает ли Microsoft Excel точки данных от последней к первой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Представляет положение меток делений на указанной оси.

Смотрите [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Представляет количество категорий или рядов между метками делений. Применяется только к категориальным и рядовым осям.

**Remarks**

Число должно быть от 1 до 31999.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Возвращает или задает количество категорий или рядов между делениями. Применяется только к категориальным и рядовым осям.

**Remarks**

Число должно быть от 1 до 31999.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Представляет, видна ли ось.

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

