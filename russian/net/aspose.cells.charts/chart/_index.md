---
title: Chart
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий одну диаграмму Excel.
type: docs
weight: 430
url: /ru/net/aspose.cells.charts/chart/
---
## Chart class

Инкапсулирует объект, представляющий одну диаграмму Excel.

```csharp
public class Chart
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | Истинно, если Microsoft Excel масштабирует трехмерную диаграмму так, чтобы ее размер был ближе к эквивалентной двухмерной диаграмме. Свойство RightAngleAxes должно иметь значение True. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Возвращает объект[`Walls`](./walls), представляющий заднюю стенку трехмерной диаграммы. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Получает ось X графика. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Получает область диаграммы на листе. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Представляет таблицу данных диаграммы. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | Представляет chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Представляет глубину трехмерной диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Указывает, отображается ли #N/A как пустое значение. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Представляет высоту трехмерной карты в градусах. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Получает или задает угол первого среза круговой или кольцевой диаграммы в градусах (от вертикали по часовой стрелке). Применяется только к круговым, трехмерным круговым и кольцевым диаграммам от 0 до 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Возвращает объект[`Floor`](./floor), представляющий стены трехмерной диаграммы. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Получает или задает расстояние между рядами данных на трехмерной диаграмме в процентах от ширины маркера. Значение этого свойства должно быть между 0 и 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Возвращает или задает расстояние между кластерами столбцов или столбцов в процентах от ширины столбца или столбца. Значение этого свойства должно быть между 0 и 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Возвращает или задает высоту трехмерной диаграммы в процентах от ширины диаграммы (от 5 до 500 процентов). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Указывает, следует ли скрывать кнопки поля сводной диаграммы только в том случае, если диаграмма является сводной диаграммой. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Указывает, является ли диаграмма трехмерной. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Получает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. Значение по умолчанию — true. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Получает легенду диаграммы. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Получает строку. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Получает и задает имя диаграммы. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | Получает коллекцию[`SeriesCollection`](../seriescollection), представляющую серию данных на диаграмме. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Представляет описание настройки страницы на этой диаграмме. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Возвращает или задает перспективу для просмотра трехмерной диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes имеет значение True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Определяет элементы управления поворотом, которые появляются на графике |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | Источником являются данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Представляет способ прикрепления диаграммы к ячейкам под ней. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Получает область построения диаграммы, которая включает метки делений осей. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Получает и задает график по строке или по столбцу. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Получает и задает способ построения пустых ячеек. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Указывает, отображать ли на графике только видимые ячейки. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Получает и задает размер распечатываемой диаграммы. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Истинно, если оси диаграммы расположены под прямым углом. Применяется только для трехмерных диаграмм (кроме Column3D и трехмерных круговых диаграмм). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Представляет поворот представления трехмерной диаграммы (поворот области графика вокруг оси Z в градусах). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Получает вторую ось X диаграммы. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Получает вторую ось Y диаграммы. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Получает ось серии диаграммы. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Возвращает все фигуры рисунка на этой диаграмме. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Получает или задает значение, указывающее, отображает ли диаграмма таблицу данных. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Получает или задает значение, указывающее, будет ли отображаться легенда диаграммы. Значение по умолчанию верно. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Возвращает объект[`Walls`](./walls), представляющий боковую стенку трехмерной диаграммы. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Истинно, если Microsoft Excel изменяет размер диаграммы, чтобы она соответствовала размеру окна листа диаграммы. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Получает и устанавливает встроенный стиль. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Получает подзаголовок диаграммы. Только для файла формата ODS. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Получает заголовок диаграммы. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Получает или задает тип диаграммы. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Получает ось Y графика. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Возвращает объект[`Walls`](./walls), представляющий стены трехмерной диаграммы. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Истинно, если линии сетки нарисованы двумерными на трехмерной диаграмме. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Получает рабочий лист, содержащий эту диаграмму. |

## Методы

| Имя | Описание |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Вычисляет произвольное положение области графика, осей, если их положение назначено автоматически. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Получает реальный размер диаграммы в пикселях. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Получает диапазон источника данных диаграммы. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Возвращает, какие оси существуют на графике. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Определяет, изменился ли источник данных диаграммы. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Перемещает диаграмму в указанное место. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Обновляет данные сводной диаграммы из ее источника данных. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Указывает диапазон данных для диаграммы. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Переключает строку/столбец. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Получает 32-битный` Bitmap` объект графика. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Получает 32-битный` Bitmap` объект графика. ` ImageOrPrintOptions.ImageFormat` , Атрибуты ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality игнорируются. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_5)(string) | Создает изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, ImageFormat) | Создает изображение графика и сохраняет его в потоке в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageOrPrintOptions) | Создает изображение графика и сохраняет его в потоке в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, long) | Создает изображение графика и сохраняет его в поток в формате Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageFormat) | Создает изображение графика и сохраняет его в файл в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string, ImageOrPrintOptions) | Создает изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, long) | Создает изображение графика и сохраняет его в файл в формате Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Создает диаграмму в формате pdf и сохраняет ее в поток. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Сохраняет диаграмму в файл pdf. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Создает диаграмму в формате pdf и сохраняет ее в поток. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Сохраняет диаграмму в файл pdf. |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Смотрите также

* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
