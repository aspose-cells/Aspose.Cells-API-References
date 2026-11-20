---
title: "Диаграмма"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий отдельную диаграмму Excel."
type: docs
url: /ru/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Инкапсулирует объект, представляющий отдельную диаграмму Excel.

**Example**

Следующий код показывает, как создать диаграмму с помощью кода .NET.

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Методы

| Метод | Описание |
| --- | --- |
| [calculate()](#calculate--) | Вычисляет пользовательские позиции области построения и осей, если их позиции назначаются автоматически. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Вычисляет пользовательскую позицию области построения и осей, если их позиции назначаются автоматически, с параметрами расчёта диаграммы. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Изменить тип диаграммы с помощью предустановленного шаблона. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Получает фактический размер диаграммы в пикселях. |
| [getActualSize()](#getActualSize--) | Получает фактический размер диаграммы в пикселях. |
| [getAutoScaling()](#getAutoScaling--) | True, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. |
| [getBackWall()](#getBackWall--) | Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--), представляющий заднюю стенку 3‑D диаграммы. |
| [getCategoryAxis()](#getCategoryAxis--) | Получает ось X диаграммы. |
| [getChartArea()](#getChartArea--) | Получает область диаграммы в листе. |
| [getChartDataRange()](#getChartDataRange--) | Получает диапазон источника данных диаграммы. |
| [getChartDataTable()](#getChartDataTable--) | Представляет таблицу данных диаграммы. |
| [getChartObject()](#getChartObject--) | Представляет chartShape; |
| [getChartShape()](#getChartShape--) | Представляет chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Указывает, следует ли отображать \#N/A как пустое значение. |
| [getElevation()](#getElevation--) | Представляет угол наклона 3‑D представления диаграммы в градусах. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Получает коллекцию [SeriesCollection](../../com.aspose.cells/seriescollection), представляющую серии данных, отфильтрованные в диаграмме. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Получает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). |
| [getFloor()](#getFloor--) | Возвращает объект [getFloor()](../../com.aspose.cells/chart\#getFloor--), представляющий стены 3‑D диаграммы. |
| [getGapDepth()](#getGapDepth--) | Получает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. |
| [getGapWidth()](#getGapWidth--) | Возвращает или задает интервал между кластерами столбцов или колонок в процентах от их ширины. |
| [getHeightPercent()](#getHeightPercent--) | Возвращает или задает высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 процентов). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart. |
| [getIs3D()](#getIs3D--) | Указывает, является ли диаграмма 3‑D. |
| [getLegend()](#getLegend--) | Получает легенду диаграммы. |
| [getLine()](#getLine--) | Получает линию. |
| [getNSeries()](#getNSeries--) | Получает коллекцию [SeriesCollection](../../com.aspose.cells/seriescollection), представляющую серии данных в диаграмме. |
| [getName()](#getName--) | Получает имя диаграммы. |
| [getPageSetup()](#getPageSetup--) | Представляет описание настройки страницы в этой диаграмме. |
| [getPerspective()](#getPerspective--) | Возвращает или задает перспективу для трех\\u9225\\u6178мерного представления диаграммы. |
| [getPivotOptions()](#getPivotOptions--) | Указывает элементы управления сводной таблицей, которые отображаются на диаграмме. |
| [getPivotSource()](#getPivotSource--) | Источник — данные сводной таблицы. |
| [getPlacement()](#getPlacement--) | Представляет способ привязки диаграммы к ячейкам под ней. |
| [getPlotArea()](#getPlotArea--) | Получает область построения диаграммы, включающую подписи делений осей. |
| [getPlotBy()](#getPlotBy--) | Получает, построен ли график по строке или столбцу. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Получает, как отображать пустые ячейки. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Указывает, отображать ли только видимые ячейки. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Указывает, отображать ли только видимые ячейки. |
| [getPrintSize()](#getPrintSize--) | Получает размер печатного графика. |
| [getRightAngleAxes()](#getRightAngleAxes--) | Истина, если оси графика образуют прямой угол. |
| [getRotationAngle()](#getRotationAngle--) | Представляет вращение 3‑D представления графика (вращение области построения вокруг оси Z в градусах). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Получает вторую ось X графика. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Получает вторую ось Y графика. |
| [getSeriesAxis()](#getSeriesAxis--) | Получает ось серии графика. |
| [getShapes()](#getShapes--) | Возвращает все графические фигуры в этом графике. |
| [getShowDataTable()](#getShowDataTable--) | Получает значение, указывающее, отображает ли график таблицу данных. |
| [getShowLegend()](#getShowLegend--) | Получает значение, указывающее, будет ли отображена легенда графика. |
| [getSideWall()](#getSideWall--) | Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--) , представляющий боковую стенку 3‑D графика. |
| [getSizeWithWindow()](#getSizeWithWindow--) | Истина, если Microsoft Excel изменяет размер графика, чтобы он соответствовал размеру окна листа графика. |
| [getStyle()](#getStyle--) | Получает встроенный стиль. |
| [getSubTitle()](#getSubTitle--) | Получает подзаголовок графика. |
| [getTitle()](#getTitle--) | Получает заголовок графика. |
| [getType()](#getType--) | Получает тип графика. |
| [getValueAxis()](#getValueAxis--) | Получает ось Y графика. |
| [getWalls()](#getWalls--) | Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--) , представляющий стены 3‑D графика. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | Истина, если линии сетки рисуются в двумерном виде на 3‑D графике. |
| [getWorksheet()](#getWorksheet--) | Получает лист, содержащий этот график. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Возвращает, какие оси присутствуют на графике. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Возвращает, относится ли ячейка к графику. |
| [isChartDataChanged()](#isChartDataChanged--) | Определяет, изменился ли источник данных диаграммы. |
| [isRectangularCornered()](#isRectangularCornered--) | Получает значение, указывающее, имеет ли область диаграммы прямоугольные углы. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Возвращает, ссылается ли ячейка на диаграмму. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Перемещает диаграмму в указанное место. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Обновляет данные диаграммы из сводной таблицы. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | True, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Указывает диапазон данных для диаграммы. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Указывает, следует ли отображать \#N/A как пустое значение. |
| [setElevation(int value)](#setElevation-int-) | Представляет угол наклона 3‑D представления диаграммы в градусах. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Устанавливает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). |
| [setGapDepth(int value)](#setGapDepth-int-) | Устанавливает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. |
| [setGapWidth(int value)](#setGapWidth-int-) | Возвращает или задает интервал между кластерами столбцов или колонок в процентах от их ширины. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Возвращает или задает высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 процентов). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя диаграммы. |
| [setPerspective(short value)](#setPerspective-short-) | Возвращает или задает перспективу для трех\\u9225\\u6178мерного представления диаграммы. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | Источник — данные сводной таблицы. |
| [setPlacement(int value)](#setPlacement-int-) | Представляет способ привязки диаграммы к ячейкам под ней. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Устанавливает способ отображения пустых ячеек. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Указывает, отображать ли только видимые ячейки. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Указывает, отображать ли только видимые ячейки. |
| [setPrintSize(int value)](#setPrintSize-int-) | Устанавливает размер печатной диаграммы. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Устанавливает значение, указывающее, имеет ли область диаграммы прямоугольные углы. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | Истина, если оси графика образуют прямой угол. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Представляет вращение 3‑D представления графика (вращение области построения вокруг оси Z в градусах). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Устанавливает значение, указывающее, отображает ли диаграмма таблицу данных. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Устанавливает значение, указывающее, будет ли отображена легенда диаграммы. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | Истина, если Microsoft Excel изменяет размер графика, чтобы он соответствовал размеру окна листа графика. |
| [setStyle(int value)](#setStyle-int-) | Устанавливает встроенный стиль. |
| [setType(int value)](#setType-int-) | Устанавливает тип диаграммы. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | Истина, если линии сетки рисуются в двумерном виде на 3‑D графике. |
| [switchRowColumn()](#switchRowColumn--) | Переключает строки/столбцы. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Создаёт изображение диаграммы и сохраняет его в файл. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Создаёт изображение диаграммы и сохраняет его в файл в указанном формате. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Создаёт изображение диаграммы и сохраняет его в файл. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Создаёт изображение диаграммы и сохраняет его в файл в указанном типе изображения. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Создаёт изображение диаграммы и сохраняет его в файл в формате JPEG. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Создаёт PDF‑файл диаграммы и сохраняет его в поток. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Создаёт PDF‑файл диаграммы и сохраняет его в поток. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Сохраняет диаграмму в PDF‑файл. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Сохраняет диаграмму в PDF‑файл. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Вычисляет пользовательские позиции области построения и осей, если их позиции назначаются автоматически.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Вычисляет пользовательскую позицию области построения и осей, если их позиции назначаются автоматически, с параметрами расчёта диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Изменить тип диаграммы с помощью предустановленного шаблона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| данные | byte[] | Данные файла шаблона диаграммы (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Получает фактический размер диаграммы в пикселях.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте метод Chart.getActualSize(). Это свойство будет удалено через 12 месяцев, начиная с июля 2022 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Returns:**
int[] — Фактический размер в массиве (ширина и высота). [0] — ширина; [1] — высота.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Получает фактический размер диаграммы в пикселях.

**Returns:**
int[] — Фактический размер в массиве (ширина и высота). [0] — ширина; [1] — высота.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


True, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. Свойство RightAngleAxes должно быть True.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--), представляющий заднюю стенку 3‑D диаграммы.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Получает ось X диаграммы.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Получает область диаграммы в листе.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Получает диапазон источника данных диаграммы.

**Remarks**

Поддерживается только диапазон. Если Series.Values, Name и XValues находятся в непрерывном диапазоне, будет возвращён диапазон, содержащий их.

**Returns:**
java.lang.String — Источник данных.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Представляет таблицу данных диаграммы.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Представляет chartShape;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Представляет chartShape;

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Charts.Chart.ChartObject. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Указывает, следует ли отображать \#N/A как пустое значение.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Представляет угол наклона 3‑D представления диаграммы в градусах.

**Remarks**

Высота диаграммы — это высота, с которой вы просматриваете диаграмму, в градусах. По умолчанию 15 для большинства типов диаграмм. Значение этого свойства должно быть от -90 до 90, за исключением 3‑D столбчатых диаграмм, где оно должно быть от 0 до 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Получает коллекцию [SeriesCollection](../../com.aspose.cells/seriescollection), представляющую серии данных, отфильтрованные в диаграмме.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Возвращает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, от 0 до 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Возвращает объект [getFloor()](../../com.aspose.cells/chart\#getFloor--), представляющий стены 3‑D диаграммы.

**Remarks**

Это свойство не применяется к 3‑D круговым диаграммам.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Возвращает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. Значение этого свойства должно быть от 0 до 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Возвращает или задаёт пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Возвращает или задает высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 процентов).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Указывает, является ли диаграмма 3‑D.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Получает легенду диаграммы.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Получает линию.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Получает коллекцию [SeriesCollection](../../com.aspose.cells/seriescollection), представляющую серии данных в диаграмме.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Получает имя диаграммы.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Представляет описание настройки страницы в этой диаграмме.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Возвращает или задаёт перспективу для трёхмерного вида диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes равно True.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Указывает элементы управления сводной таблицей, которые отображаются на диаграмме.

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart.

**Remarks**

Если сводная таблица "PivotTable1" находится на листе "Sheet1" в файле "Book1.xls". pivotSource может быть "[Book1.xls]Sheet1!PivotTable1", если диаграмма и сводная таблица находятся в разных рабочих книгах. Если вы зададите это свойство, предыдущая настройка источника данных будет потеряна.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Представляет способ привязки диаграммы к ячейкам под ней.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Получает область построения диаграммы, включающую подписи делений осей.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Получает, построен ли график по строке или столбцу.

Смотрите [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Получает, как отображать пустые ячейки.

См. [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Указывает, отображать ли только видимые ячейки.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotVisibleCellsOnly. Этот метод будет удалён через 12 месяцев, начиная с декабря 2022 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Указывает, отображать ли только видимые ячейки.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Получает размер печатного графика.

Смотрите [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


True, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм).

**Remarks**

Если это свойство равно True, свойство Perspective игнорируется.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Представляет вращение 3‑D представления графика (вращение области построения вокруг оси Z в градусах).

**Remarks**

Значение этого свойства должно быть от 0 до 360, за исключением 3‑D столбчатых диаграмм, где значение должно быть от 0 до 44. Значение по умолчанию — 20. Применяется только к 3‑D диаграммам.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Получает вторую ось X графика.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Получает вторую ось Y графика.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Получает ось серии графика.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Возвращает все графические фигуры в этом графике.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Получает значение, указывающее, отображает ли график таблицу данных.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Возвращает значение, указывающее, будет ли отображаться легенда диаграммы. По умолчанию true.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--) , представляющий боковую стенку 3‑D графика.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


Истина, если Microsoft Excel изменяет размер графика, чтобы он соответствовал размеру окна листа графика.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Получает встроенный стиль.

**Remarks**

Должно быть от 1 до 48. Возвращает -1, если не установлено.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Возвращает подзаголовок диаграммы. Применяется только к ODS‑файлам.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Получает заголовок графика.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Получает тип графика.

Смотрите [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Получает ось Y графика.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Возвращает объект [getWalls()](../../com.aspose.cells/chart\#getWalls--) , представляющий стены 3‑D графика.

**Remarks**

Это свойство не применяется к 3‑D круговым диаграммам.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


Истина, если линии сетки рисуются в двумерном виде на 3‑D графике.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает лист, содержащий этот график.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Возвращает, какие оси присутствуют на графике.

**Remarks**

Обычно, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded не имеет оси.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Возвращает, относится ли ячейка к графику.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа. -1 означает лист, содержащий текущую диаграмму. |
| rowIndex | int | Индекс строки |
| columnIndex | int | Индекс столбца |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Определяет, изменился ли источник данных диаграммы.

**Remarks**

Метод обнаруживает изменения в источнике данных диаграммы перед рендерингом диаграммы в формат изображения. При первом вызове Chart.toImage исходные данные диаграммы (например, XValuesParseData, ValuesParseData) будут записаны. Перед повторным вызовом метода Chart.toImage вызовите метод IsChartDataChanged, чтобы проверить, требуется ли повторный рендеринг диаграммы.

**Returns:**
boolean - Возвращает true, если диаграмма изменилась, иначе возвращает false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Получает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Возвращает, ссылается ли ячейка на диаграмму.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод IsCellReferedByChart(int,int,int). Этот метод будет удалён через 12 месяцев, начиная с апреля 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки |
| columnIndex | int | Индекс столбца |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Перемещает диаграмму в указанное место.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| bottomRow | int | Индекс строки в нижнем правом углу |
| rightColumn | int | Индекс столбца в нижнем правом углу |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Обновляет данные диаграммы из сводной таблицы.

**Remarks**

Мы соберём данные из источника сводных данных в отчёт сводной таблицы. Этот метод используется только для сбора всех данных в сводную диаграмму.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


True, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. Свойство RightAngleAxes должно быть True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Указывает диапазон данных для диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | java.lang.String | Указывает значения, из которых строятся ряды данных |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Указывает, следует ли отображать \#N/A как пустое значение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Представляет угол наклона 3‑D представления диаграммы в градусах.

**Remarks**

Высота диаграммы — это высота, с которой вы просматриваете диаграмму, в градусах. По умолчанию 15 для большинства типов диаграмм. Значение этого свойства должно быть от -90 до 90, за исключением 3‑D столбчатых диаграмм, где оно должно быть от 0 до 44.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Устанавливает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, диапазон 0–360.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Устанавливает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. Значение этого свойства должно быть от 0 до 500.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Возвращает или задаёт пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Возвращает или задает высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 процентов).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Возвращает или задаёт перспективу для трёхмерного вида диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes равно True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart.

**Remarks**

Если сводная таблица "PivotTable1" находится на листе "Sheet1" в файле "Book1.xls". pivotSource может быть "[Book1.xls]Sheet1!PivotTable1", если диаграмма и сводная таблица находятся в разных рабочих книгах. Если вы зададите это свойство, предыдущая настройка источника данных будет потеряна.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Представляет способ привязки диаграммы к ячейкам под ней.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Устанавливает способ отображения пустых ячеек.

См. [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Указывает, отображать ли только видимые ячейки.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotVisibleCellsOnly. Этот метод будет удалён через 12 месяцев, начиная с декабря 2022 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Указывает, отображать ли только видимые ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Устанавливает размер печатной диаграммы.

Смотрите [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Устанавливает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


True, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм).

**Remarks**

Если это свойство равно True, свойство Perspective игнорируется.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Представляет вращение 3‑D представления графика (вращение области построения вокруг оси Z в градусах).

**Remarks**

Значение этого свойства должно быть от 0 до 360, за исключением 3‑D столбчатых диаграмм, где значение должно быть от 0 до 44. Значение по умолчанию — 20. Применяется только к 3‑D диаграммам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Устанавливает значение, указывающее, отображает ли диаграмма таблицу данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Устанавливает значение, указывающее, будет ли отображаться легенда диаграммы. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


Истина, если Microsoft Excel изменяет размер графика, чтобы он соответствовал размеру окна листа графика.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Устанавливает встроенный стиль.

**Remarks**

Должно быть от 1 до 48. Возвращает -1, если не установлено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип диаграммы.

Смотрите [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


Истина, если линии сетки рисуются в двумерном виде на 3‑D графике.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Переключает строки/столбцы.

**Returns:**
boolean - False означает, что переключение строк/столбцов не удалось.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Создаёт изображение диаграммы и сохраняет его в поток в указанном формате.

**Remarks**

Формат изображения задаётся с помощью `options.ImageFormat`. Поддерживаются следующие форматы: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Если ширина или высота равны нулю, либо диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. Пожалуйста, обратитесь к [Supported Charts List][] для получения более подробной информации.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток вывода. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Дополнительные параметры создания изображения |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

**Remarks**

Формат изображения задаётся с помощью расширения имени файла. Например, если указать "myfile.png", изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю, либо диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String | Имя файла изображения с полным путём. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Создаёт изображение диаграммы и сохраняет его в файл в указанном формате.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте метод Chart.ToImage(string, ImageType). Это свойство будет удалено через 12 месяцев, начиная с июля 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String | Имя файла изображения с полным путём. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Формат, в котором сохранять изображение. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

**Remarks**

Формат изображения задаётся с помощью расширения имени файла. Например, если указать "myfile.png", изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю, либо диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. Пожалуйста, обратитесь к [Supported Charts List][] для получения более подробной информации.

**Example**

Сохраняет в Tiff с разрешением 300 dpi и сжатие CCITT4.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String | Имя файла изображения с полным путём. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Дополнительные параметры создания изображения |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Создаёт изображение диаграммы и сохраняет его в файл в указанном типе изображения.

**Remarks**

Тип изображения указывается с помощью `imageType`. Поддерживаются следующие типы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю, либо диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String | Имя файла изображения с полным путём. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Тип изображения, в котором сохранять изображение. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Создаёт изображение диаграммы и сохраняет его в файл в формате JPEG.

**Remarks**

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод ToImage(string,ImageOrPrintOptions) с указанным качеством. Этот метод будет удалён через 12 месяцев, начиная с марта 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String | Имя файла изображения с полным путём. |
| jpegQuality | long | Качество JPEG. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Создаёт PDF‑файл диаграммы и сохраняет его в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток вывода. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Создаёт PDF‑файл диаграммы и сохраняет его в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток вывода. |
| desiredPageWidth | float | Желаемая ширина страницы в дюймах. |
| desiredPageHeight | float | Желаемая высота страницы в дюймах. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Горизонтальный тип выравнивания диаграммы на выходной странице. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Вертикальный тип выравнивания диаграммы на выходной странице. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Сохраняет диаграмму в PDF‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | полное имя PDF‑файла с полным путём |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Сохраняет диаграмму в PDF‑файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | полное имя PDF‑файла с полным путём |
| desiredPageWidth | float | Желаемая ширина страницы в дюймах. |
| desiredPageHeight | float | Желаемая высота страницы в дюймах. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Горизонтальный тип выравнивания диаграммы на выходной странице. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Вертикальный тип выравнивания диаграммы на выходной странице. |

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

