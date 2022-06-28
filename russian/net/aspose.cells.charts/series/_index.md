---
title: Series
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий один ряд данных на диаграмме.
type: docs
weight: 820
url: /ru/net/aspose.cells.charts/series/
---
## Series class

Инкапсулирует объект, представляющий один ряд данных на диаграмме.

```csharp
public class Series
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area) { get; } | Представляет фоновую область объекта Series. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype) { get; set; } | Получает или задает тип трехмерной фигуры, используемый с трехмерной гистограммой или гистограммой. |
| [Border](../../aspose.cells.charts/series/border) { get; } | Представляет границу объекта серии. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale) { get; set; } | Получает или задает коэффициент масштабирования для пузырьков в указанной группе диаграммы. Это может быть целочисленное значение от 0 (ноль) до 300, соответствующее проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes) { get; set; } | Получает или задает значения размеров пузырьков ряда диаграммы. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues) { get; } | Получает количество значений данных. |
| [DataLabels](../../aspose.cells.charts/series/datalabels) { get; } | Представляет объект DataLabels для указанного ASeries. |
| [DisplayName](../../aspose.cells.charts/series/displayname) { get; } | Получает имя серии, которое отображается на графике диаграммы. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize) { get; set; } | Возвращает или задает размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы в диапазоне от 10 до 90 процентов. |
| [DownBars](../../aspose.cells.charts/series/downbars) { get; } | Возвращает объект[`DropBars`](../dropbars), представляющий нижние бары на линейной диаграмме. Применяется только к линейным графикам. |
| [DropLines](../../aspose.cells.charts/series/droplines) { get; } | Возвращает объект[`Line`](../../aspose.cells.drawing/line), представляющий перетаскиваемые линии для ряда на линейной диаграмме или диаграмме с областями. . Применяется только к линейным диаграммам или диаграммам с областями. |
| [Explosion](../../aspose.cells.charts/series/explosion) { get; set; } | Расстояние открытого сектора круговой диаграммы от центра круговой диаграммы выражается в процентах от диаметра круговой диаграммы. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle) { get; set; } | Получает или задает угол первого среза круговой или кольцевой диаграммы в градусах (от вертикали по часовой стрелке). Применяется только к круговым, трехмерным круговым и кольцевым диаграммам, от 0 до 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth) { get; set; } | Возвращает или задает расстояние между кластерами столбцов или столбцов в процентах от ширины столбца или столбца. Значение этого свойства должно быть между 0 и 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect) { get; set; } | Истинно, если серия имеет трехмерный вид. Применяется только к пузырьковым диаграммам. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines) { get; set; } | Истинно, если на диаграмме есть перетаскиваемые линии. Применяется только к линейным диаграммам или диаграммам с областями. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines) { get; set; } | Истинно, если на линейном графике есть линии максимума-минимума. Применяется только к линейным графикам. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines) { get; set; } | Истинно, если ряд имеет линии выноски. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels) { get; set; } | Истинно, если лепестковая диаграмма имеет метки оси категорий. Применяется только к радиолокационным картам. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines) { get; set; } | Истинно, если столбчатая диаграмма с накоплением или столбчатая диаграмма имеет линии серий или если круговая диаграмма или столбчатая диаграмма имеет соединительные линии между две секции. Применяется только к столбчатым диаграммам с накоплением, столбчатым диаграммам, круговым диаграммам или столбчатым диаграммам. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars) { get; set; } | Истинно, если линейный график имеет столбцы вверх и вниз. Применяется только к линейным графикам. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines) { get; } | Возвращает объект HiLoLines, который представляет линии максимума и минимума для ряда на линейной диаграмме. Применяется только к линейным графикам. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit) { get; } | Указывает, является ли пороговое значение автоматическим. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried) { get; set; } | Указывает, различаются ли цвета точек. Диаграмма должна содержать только одну серию. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues) { get; } | Указывает, является ли источник данных вертикальным. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties) { get; } | Представляет свойства макета. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines) { get; } | Представляет линии выноски на графике. Линии выноски соединяют метки данных с точками данных. Этот объект не является коллекцией; нет объекта, представляющего одну линию выноски. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry) { get; } | Получает запись легенды в соответствии с этой серией. |
| [Marker](../../aspose.cells.charts/series/marker) { get; } | Получает[`marker`](./marker) . |
| [Name](../../aspose.cells.charts/series/name) { get; set; } | Получает или задает имя ряда данных. |
| [Overlap](../../aspose.cells.charts/series/overlap) { get; set; } | Указывает, как позиционируются полосы и столбцы. Может быть значением от – 100 до 100. Применяется только к двухмерным гистограммам и двумерным столбчатым диаграммам. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis) { get; set; } | Указывает, нанесен ли этот ряд на вторую ось значений. |
| [Points](../../aspose.cells.charts/series/points) { get; } | Получает набор точек в серии на диаграмме. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize) { get; set; } | Возвращает или задает размер вторичной части круговой диаграммы или столбца круговой диаграммы, в процентах от размер основного пирога. Может принимать значение от 5 до 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines) { get; } | Возвращает объект SeriesLines, который представляет строки ряда для гистограммы с накоплением или гистограммы с накоплением. Применяется только к линейчатым и столбчатым диаграммам с накоплением. |
| [Shadow](../../aspose.cells.charts/series/shadow) { get; set; } | Истинно, если серия имеет тень. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties) { get; } | Получает объект, содержащий свойства визуальной формы серии. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles) { get; set; } | Истинно, если для группы диаграммы отображаются отрицательные кружки. Действительно только для пузырьковых диаграмм. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents) { get; set; } | Получает или задает значение размера пузырька на пузырьковой диаграмме. |
| [Smooth](../../aspose.cells.charts/series/smooth) { get; set; } | Представляет сглаживание кривой. True, если сглаживание кривых включено для линейной диаграммы или точечной диаграммы. Применяется только к линейным и точечным графикам, связанным линиями. |
| [SplitType](../../aspose.cells.charts/series/splittype) { get; set; } | Возвращает или задает значение, позволяющее определить, какие точки данных находятся во втором круге или столбце круга или столбце круга диаграмма. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue) { get; set; } | Возвращает или задает значение, которое будет использоваться для определения того, какие точки данных находятся во второй круговой диаграмме или столбце на круговом круге или столбце круговой диаграммы. |
| [TrendLines](../../aspose.cells.charts/series/trendlines) { get; } | Возвращает объект, представляющий набор всех линий тренда для ряда. |
| [Type](../../aspose.cells.charts/series/type) { get; set; } | Получает или задает тип ряда данных. |
| [UpBars](../../aspose.cells.charts/series/upbars) { get; } | Возвращает объект DropBars, представляющий восходящие бары на линейном графике. Применяется только к линейным графикам. |
| [Values](../../aspose.cells.charts/series/values) { get; set; } | Представляет данные ряда диаграммы. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode) { get; set; } | Представляет код формата списка номеров значений. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar) { get; } | Представляет линейку погрешностей направления X ряда. |
| [XValues](../../aspose.cells.charts/series/xvalues) { get; set; } | Представляет значения x серии диаграммы. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar) { get; } | Представляет линейку погрешностей направления Y ряда. |

## Методы

| Имя | Описание |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move)(int) | Перемещает серию вверх или вниз. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  //Добавление нового рабочего листа в Excel object
int sheetIndex = workbook.Worksheets.Add();
  //Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
  //Добавление значения выборки в "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Добавление значения образца в "A2" cell
worksheet.Cells["A2"].PutValue(100);
  //Добавление значения образца в "A3" cell
worksheet.Cells["A3"].PutValue(150);
  //Добавление образца значения в "A4" cell
worksheet.Cells["A4"].PutValue(200);
  //Добавление образца значения в "B1" cell
worksheet.Cells["B1"].PutValue(60);
  //Добавление значения образца в "B2" cell
worksheet.Cells["B2"].PutValue(32);
  //Добавление значения образца в "B3" cell
worksheet.Cells["B3"].PutValue(50);
  //Добавление значения образца в "B4" cell
worksheet.Cells["B4"].PutValue(40);
  //Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells["C1"].PutValue("Q1");
  //Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells["C2"].PutValue("Q2");
  //Добавление значения образца в ячейку "C3" как категория data
worksheet.Cells["C3"].PutValue("Y1");
  //Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells["C4"].PutValue("Y2");
  //Добавление диаграммы на лист
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
  //Доступ к экземпляру только что добавленного chart
Chart chart = worksheet.Charts[chartIndex];
  //Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
  //Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
  //Установка значений ряда.
series.Values = "=B1:B4";
  //Изменяем тип графика серии.
series.Type = ChartType.Line;
  //Установка свойств маркера.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

  //делай свое дело

  //Сохранение файла Excel
workbook.Save("book1.xls");

[Visual Basic]

'Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()
'Добавление нового рабочего листа в Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Добавление значения выборки в "A1" cell
worksheet.Cells("A1").PutValue(50)
'Добавление значения выборки в "A2" cell
worksheet.Cells("A2").PutValue(100)
'Добавление значения выборки в "A3" cell
worksheet.Cells("A3").PutValue(150)
'Добавление значения выборки в "A4" cell
worksheet.Cells("A4").PutValue(200)
'Добавление образца значения в "B1" cell
worksheet.Cells("B1").PutValue(60)
'Добавление образца значения в "B2" cell
worksheet.Cells("B2").PutValue(32)
'Добавление образца значения в "B3" cell
worksheet.Cells("B3").PutValue(50)
'Добавление образца значения в "B4" cell
worksheet.Cells("B4").PutValue(40)
'Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells("C1").PutValue("Q1")
'Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells("C2").PutValue("Q2")
'Добавление образца значения в ячейку "C3" как категория data
worksheet.Cells("C3").PutValue("Y1")
'Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells("C4").PutValue("Y2")
'Добавление диаграммы на лист
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Доступ к экземпляру только что добавленного chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'Установка значений ряда.
series.Values = "=B1:B4"
'Изменение типа диаграммы ряда.
series.Type = ChartType.Line
'Настройка свойств маркера.
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'Сохранение файла Excel
workbook.Save("book1.xls")
```

### Смотрите также

* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
