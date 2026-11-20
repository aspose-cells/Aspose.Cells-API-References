---
title: "Series"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий одну серию данных в диаграмме."
type: docs
url: /ru/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Инкапсулирует объект, представляющий одну серию данных в диаграмме.

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
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Представляет фоновую область объекта Series. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Получает тип 3D‑формы, используемый в 3‑D гистограмме или столбчатой диаграмме. |
| [getBorder()](#getBorder--) | Представляет границу объекта Series. |
| [getBubbleScale()](#getBubbleScale--) | Получает коэффициент масштабирования пузырей в указанной группе диаграммы. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Получает, что представляет размер пузыря на пузырьковой диаграмме. |
| [getBubbleSizes()](#getBubbleSizes--) | Получает значения размеров пузырей серии диаграммы. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Получает кэшированные значения категорий для серии |
| [getCachedValues()](#getCachedValues--) | Получает кэшированные значения для серии |
| [getCategoryValues()](#getCategoryValues--) | Получает фактические значения категорий, используемые для построения каждой точки этой серии в диаграмме. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Получает количество значений данных. |
| [getDataLabels()](#getDataLabels--) | Представляет объект DataLabels для указанного ASeries. |
| [getDisplayName()](#getDisplayName--) | Получает имя серии, отображаемое на графике диаграммы. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Возвращает или задает размер отверстия в группе кольцевой диаграммы. |
| [getDownBars()](#getDownBars--) | Возвращает объект [DropBars](../../com.aspose.cells/dropbars), представляющий нижние бары на линейной диаграмме. |
| [getDropLines()](#getDropLines--) | Возвращает объект [Line](../../com.aspose.cells/line), представляющий линии падения для серии на линейной или площадной диаграмме. |
| [getExplosion()](#getExplosion--) | Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Получает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). |
| [getGapWidth()](#getGapWidth--) | Возвращает или задает интервал между кластерами столбцов или колонок в процентах от их ширины. |
| [getHas3DEffect()](#getHas3DEffect--) | True, если у серии трехмерный вид. |
| [getHiLoLines()](#getHiLoLines--) | Возвращает объект HiLoLines, представляющий линии high‑low для серии на линейной диаграмме. |
| [getLayoutProperties()](#getLayoutProperties--) | Представляет свойства макета. |
| [getLeaderLines()](#getLeaderLines--) | Представляет направляющие линии на диаграмме. |
| [getLegendEntry()](#getLegendEntry--) | Получает запись легенды, соответствующую этой серии. |
| [getMarker()](#getMarker--) | Получает [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Получает имя серии данных. |
| [getOverlap()](#getOverlap--) | Указывает, как позиционируются столбцы и полосы. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Указывает, построен ли этот ряд на второй оси значений. |
| [getPointValues()](#getPointValues--) | Получает фактические значения, используемые для построения каждой точки этого ряда на диаграмме. |
| [getPoints()](#getPoints--) | Получает коллекцию точек в ряду диаграммы. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Возвращает или задает размер вторичной секции диаграммы «круг в круге» или «полоса в круге» в процентах от размера основного круга. |
| [getSeriesLines()](#getSeriesLines--) | Возвращает объект SeriesLines, представляющий линии рядов для сложенной гистограммы или сложенной столбчатой диаграммы. |
| [getShadow()](#getShadow--) | True, если у ряда есть тень. |
| [getShapeProperties()](#getShapeProperties--) | Получает объект [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection), содержащий визуальные свойства формы ряда. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | True, если для группы диаграммы отображаются отрицательные пузырьки. |
| [getSizeRepresents()](#getSizeRepresents--) | Получает, что представляет размер пузыря на пузырьковой диаграмме. |
| [getSmooth()](#getSmooth--) | Представляет сглаживание кривой. |
| [getSplitType()](#getSplitType--) | Возвращает или задает значение, определяющее, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге». |
| [getSplitValue()](#getSplitValue--) | Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге». |
| [getTrendLines()](#getTrendLines--) | Возвращает все линии тренда этого ряда. |
| [getType()](#getType--) | Получает тип ряда данных. |
| [getUpBars()](#getUpBars--) | Возвращает объект DropBars, представляющий верхние бары на линейной диаграмме. |
| [getValues()](#getValues--) | Представляет значения Y этого ряда диаграммы. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Представляет код формата списка чисел Values NumberList. |
| [getXErrorBar()](#getXErrorBar--) | Представляет ошибочную полосу по оси X ряда. |
| [getXValues()](#getXValues--) | Представляет значения X этого ряда диаграммы. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Представляет код формата списка чисел X Values. |
| [getYErrorBar()](#getYErrorBar--) | Представляет ошибочную полосу по оси Y ряда. |
| [hasDropLines()](#hasDropLines--) | True, если у диаграммы есть линии спуска. |
| [hasHiLoLines()](#hasHiLoLines--) | True, если у линейной диаграммы есть линии high-low. |
| [hasLeaderLines()](#hasLeaderLines--) | True, если у ряда есть линии-выноски. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | True, если у радиальной диаграммы есть подписи оси категорий. |
| [hasSeriesLines()](#hasSeriesLines--) | Истина, если у сложенной столбчатой или гистограммной диаграммы есть линии серии, или у диаграммы «Круг в круге» или «Полоска в круге» есть соединительные линии между двумя секциями. |
| [hasUpDownBars()](#hasUpDownBars--) | Истина, если у линейной диаграммы есть верхние и нижние полосы. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Указывает, является ли значение порога автоматическим. |
| [isColorVaried()](#isColorVaried--) | Отражает, изменяется ли цвет точек. |
| [isFiltered()](#isFiltered--) | Указывает, выбран ли ряд или отфильтрован. |
| [isVerticalValues()](#isVerticalValues--) | Указывает, является ли источник данных вертикальным. |
| [move(int count)](#move-int-) | Перемещает ряд вверх или вниз. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Устанавливает тип 3D‑формы, используемой с 3‑D гистограммой или столбчатой диаграммой. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Устанавливает коэффициент масштабирования пузырей в указанной группе диаграмм. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Получает, что представляет размер пузыря на пузырьковой диаграмме. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Устанавливает значения размеров пузырей в ряду диаграммы. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Отражает, изменяется ли цвет точек. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Возвращает или задает размер отверстия в группе кольцевой диаграммы. |
| [setExplosion(int value)](#setExplosion-int-) | Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Указывает, выбран ли ряд или отфильтрован. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Устанавливает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). |
| [setGapWidth(short value)](#setGapWidth-short-) | Возвращает или задает интервал между кластерами столбцов или колонок в процентах от их ширины. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | True, если у серии трехмерный вид. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | True, если у диаграммы есть линии спуска. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | True, если у линейной диаграммы есть линии high-low. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | True, если у ряда есть линии-выноски. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | True, если у радиальной диаграммы есть подписи оси категорий. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Истина, если у сложенной столбчатой или гистограммной диаграммы есть линии серии, или у диаграммы «Круг в круге» или «Полоска в круге» есть соединительные линии между двумя секциями. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Истина, если у линейной диаграммы есть верхние и нижние полосы. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя ряда данных. |
| [setOverlap(short value)](#setOverlap-short-) | Указывает, как позиционируются столбцы и полосы. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Указывает, построен ли этот ряд на второй оси значений. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Возвращает или задает размер вторичной секции диаграммы «круг в круге» или «полоса в круге» в процентах от размера основного круга. |
| [setShadow(boolean value)](#setShadow-boolean-) | True, если у ряда есть тень. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | True, если для группы диаграммы отображаются отрицательные пузырьки. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Устанавливает, что представляет размер пузыря на пузырьковой диаграмме. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Представляет сглаживание кривой. |
| [setSplitType(int value)](#setSplitType-int-) | Возвращает или задает значение, определяющее, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге». |
| [setSplitValue(double value)](#setSplitValue-double-) | Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге». |
| [setType(int value)](#setType-int-) | Устанавливает тип ряда данных. |
| [setValues(String value)](#setValues-java.lang.String-) | Представляет значения Y этого ряда диаграммы. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Представляет код формата списка чисел Values NumberList. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Представляет значения X этого ряда диаграммы. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Представляет код формата списка чисел X Values. |
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


Представляет фоновую область объекта Series.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Получает тип 3D‑формы, используемый в 3‑D гистограмме или столбчатой диаграмме.

См. [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Представляет границу объекта Series.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Получает коэффициент масштабирования пузырей в указанной группе диаграмм. Может быть целым значением от 0 (ноль) до 300, соответствующим проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Получает, что представляет размер пузыря на пузырьковой диаграмме.

См. [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Charts.Series.SizeRepresents. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Получает значения размеров пузырей серии диаграммы.

**Remarks**

Только для [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) или [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Получает кэшированные значения категорий для серии

**Remarks**

ПРИМЕЧАНИЕ: Это свойство в настоящее время предназначено только для внутреннего использования. Оно будет изменено или удалено в следующей версии.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Получает кэшированные значения для серии

**Remarks**

ПРИМЕЧАНИЕ: Это свойство в настоящее время предназначено только для внутреннего использования. Оно будет изменено или удалено в следующей версии.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Получает фактические значения категорий, используемые для построения каждой точки этой серии в диаграмме.

**Remarks**

Это свойство предоставляет удобный способ получить фактические значения, соответствующие данным, определённым с помощью [getXValues()](../../com.aspose.cells/series\#getXValues--), особенно когда указанный источник данных является внешней ссылкой, формулой и т.д.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


Получает количество значений данных.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Представляет объект DataLabels для указанного ASeries.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Получает имя серии, отображаемое на графике диаграммы.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Возвращает или задаёт размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы, от 10 до 90 процентов.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Возвращает объект [DropBars](../../com.aspose.cells/dropbars), представляющий нижние полосы на линейной диаграмме. Применяется только к линейным диаграммам.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Возвращает объект [Line](../../com.aspose.cells/line), представляющий линии падения для ряда на линейной или областной диаграмме. Применяется только к линейным или областным диаграммам.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Получает угол первого сегмента круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, значения от 0 до 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Возвращает или задаёт пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


True, если у серии трехмерный вид.

**Remarks**

Применяется только к диаграммам [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) или [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Возвращает объект HiLoLines, представляющий линии верх‑нижнего уровня для серии на линейной диаграмме. Применяется только к линейным диаграммам.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Представляет свойства макета.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Представляет линии‑соединители на диаграмме. Линии‑соединители соединяют подписи данных с точками данных. Этот объект не является коллекцией; нет отдельного объекта, представляющего одну линию‑соединитель.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Получает запись легенды, соответствующую этой серии.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Получает [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Получает имя серии данных.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


Указывает, как позиционируются столбцы и колонки. Может принимать значение от -100 до 100. Применяется только к 2‑D гистограммам и 2‑D столбчатым диаграммам.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Указывает, построен ли этот ряд на второй оси значений.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Получает фактические значения, используемые для построения каждой точки этого ряда на диаграмме.

**Remarks**

Это свойство предоставляет удобный способ получить фактические значения, соответствующие данным, определённым методом [getValues()](../../com.aspose.cells/series\#getValues--), особенно когда указанный источник данных является внешней ссылкой, формулой и т.д.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Получает коллекцию точек в ряду диаграммы.

**Remarks**

Когда диаграмма является Pie of Pie или Bar of Pie, последняя точка — это точка «other» в первом круге.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Возвращает или задаёт размер вторичной секции диаграммы типа pie of pie или bar of pie в процентах от размера основной круговой диаграммы. Может принимать значение от 5 до 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Возвращает объект SeriesLines, представляющий линии серии для сложенной гистограммы или сложенной столбчатой диаграммы. Применяется только к сложенным гистограммам и сложенным столбчатым диаграммам.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True, если у ряда есть тень.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Получает объект [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection), содержащий визуальные свойства формы ряда.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


True, если для группы диаграмм отображаются отрицательные пузыри. Действительно только для пузырьковых диаграмм.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Получает, что представляет размер пузыря на пузырьковой диаграмме.

См. [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea означает, что значение [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) представляет площадь пузыря. BubbleSizeRepresents.SizeIsWidth означает, что значение [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) представляет ширину пузыря.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Представляет сглаживание кривой. True, если сглаживание включено для линейной диаграммы или диаграммы разброса. Применяется только к линейным диаграммам и диаграммам разброса с линиями.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Возвращает или задает значение, определяющее, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге».

Смотрите [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге».

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Возвращает все линии тренда этого ряда.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Получает тип ряда данных.

Смотрите [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Возвращает объект DropBars, представляющий верхние бары на линейной диаграмме. Применяется только к линейным диаграммам.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Представляет значения Y этого ряда диаграммы.

**Remarks**

Чтобы получить фактические значения (соответствующие каждой точке этой серии), определённые этим свойством, используйте [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Представляет код формата списка чисел Values NumberList.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Представляет ошибочную полосу по оси X ряда.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Представляет значения X этого ряда диаграммы.

**Remarks**

Только для диаграмм Scatter и Bubble. Пожалуйста, используйте [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) для других типов диаграмм; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) используется для получения фактических значений категорий этой серии.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Представляет код формата списка чисел X Values.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Представляет ошибочную полосу по оси Y ряда.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


True, если у диаграммы есть линии падения. Применяется только к линейным диаграммам или областным диаграммам.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


True, если у линейной диаграммы есть линии верх‑нижнего уровня. Применяется только к линейным диаграммам.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


True, если у ряда есть линии-выноски.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


True, если у радиальной диаграммы есть подписи оси категорий. Применяется только к радиальным диаграммам.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


True, если у сложенной столбчатой диаграммы или гистограммы есть линии серии, либо у диаграмм Pie of Pie или Bar of Pie есть соединительные линии между двумя секциями. Применяется только к сложенным столбчатым диаграммам, гистограммам, диаграммам Pie of Pie и Bar of Pie.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


True, если у линейной диаграммы есть верхние и нижние бары. Применяется только к линейным диаграммам.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


Указывает, является ли значение порога автоматическим.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Представляет, изменяется ли цвет точек. Диаграмма должна содержать только одну серию или быть круговой диаграммой.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Указывает, выбрана ли серия или отфильтрована. True означает, что эта серия отфильтрована и не будет отображаться на диаграмме.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Указывает, является ли источник данных вертикальным.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Перемещает ряд вверх или вниз.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| количество | int | Количество перемещений вверх или вниз. Переместите серию вверх, если значение меньше нуля; переместите серию вниз, если значение больше нуля. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


Устанавливает тип 3D‑формы, используемой с 3‑D гистограммой или столбчатой диаграммой.

См. [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Устанавливает коэффициент масштабирования пузырей в указанной группе диаграмм. Может быть целым значением от 0 (ноль) до 300, соответствующим проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Получает, что представляет размер пузыря на пузырьковой диаграмме.

См. [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Charts.Series.SizeRepresents. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Устанавливает значения размеров пузырей в ряду диаграммы.

**Remarks**

Только для [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) или [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Представляет, изменяется ли цвет точек. Диаграмма должна содержать только одну серию или быть круговой диаграммой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Возвращает или задаёт размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы, от 10 до 90 процентов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Указывает, выбрана ли серия или отфильтрована. True означает, что эта серия отфильтрована и не будет отображаться на диаграмме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Устанавливает угол первой части круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, значения от 0 до 360.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Возвращает или задаёт пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


True, если у серии трехмерный вид.

**Remarks**

Применяется только к диаграммам [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) или [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


True, если у диаграммы есть линии падения. Применяется только к линейным диаграммам или областным диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


True, если у линейной диаграммы есть линии верх‑нижнего уровня. Применяется только к линейным диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


True, если у ряда есть линии-выноски.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


True, если у радиальной диаграммы есть подписи оси категорий. Применяется только к радиальным диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


True, если у сложенной столбчатой диаграммы или гистограммы есть линии серии, либо у диаграмм Pie of Pie или Bar of Pie есть соединительные линии между двумя секциями. Применяется только к сложенным столбчатым диаграммам, гистограммам, диаграммам Pie of Pie и Bar of Pie.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


True, если у линейной диаграммы есть верхние и нижние бары. Применяется только к линейным диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя ряда данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Указывает, как позиционируются столбцы и колонки. Может принимать значение от -100 до 100. Применяется только к 2‑D гистограммам и 2‑D столбчатым диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Указывает, построен ли этот ряд на второй оси значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Возвращает или задаёт размер вторичной секции диаграммы типа pie of pie или bar of pie в процентах от размера основной круговой диаграммы. Может принимать значение от 5 до 200.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True, если у ряда есть тень.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


True, если для группы диаграмм отображаются отрицательные пузыри. Действительно только для пузырьковых диаграмм.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Устанавливает, что представляет размер пузыря на пузырьковой диаграмме.

См. [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea означает, что значение [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) представляет площадь пузыря. BubbleSizeRepresents.SizeIsWidth означает, что значение [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) представляет ширину пузыря.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Представляет сглаживание кривой. True, если сглаживание включено для линейной диаграммы или диаграммы разброса. Применяется только к линейным диаграммам и диаграммам разброса с линиями.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Возвращает или задает значение, определяющее, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге».

Смотрите [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во втором круге или полосе на диаграмме «круг в круге» или «полоса в круге».

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип ряда данных.

Смотрите [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Представляет значения Y этого ряда диаграммы.

**Remarks**

Чтобы получить фактические значения (соответствующие каждой точке этой серии), определённые этим свойством, используйте [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Представляет код формата списка чисел Values NumberList.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Представляет значения X этого ряда диаграммы.

**Remarks**

Только для диаграмм Scatter и Bubble. Пожалуйста, используйте [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) для других типов диаграмм; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) используется для получения фактических значений категорий этой серии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Представляет код формата списка чисел X Values.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

