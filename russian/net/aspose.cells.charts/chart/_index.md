---
title: "Класс Chart."
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Chart. Инкапсулирует объект, представляющий одну диаграмму Excel."
type: docs
url: /ru/net/aspose.cells.charts/chart/
---
## Chart class

Инкапсулирует объект, представляющий отдельную диаграмму Excel.

```csharp
public class Chart
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Возвращает фактический размер диаграммы в пикселях. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | True, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. Свойство RightAngleAxes должно быть True. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Возвращает объект [`Walls`](./walls/), представляющий заднюю стенку 3‑D диаграммы. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Получает ось X диаграммы. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Получает область диаграммы на листе. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Представляет таблицу данных диаграммы. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Представляет chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Представляет глубину 3‑D диаграммы в процентах от ширины диаграммы (от 20 до 2000 процентов). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Указывает, следует ли отображать #N/A как пустое значение. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Представляет высоту просмотра 3‑D диаграммы в градусах. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Получает коллекцию [`SeriesCollection`](../seriescollection/), представляющую серии данных, отфильтрованные в диаграмме. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, от 0 до 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Возвращает объект [`Floor`](./floor/), представляющий стены 3‑D диаграммы. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Получает или задает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера. Значение этого свойства должно быть от 0 до 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Возвращает или задает пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Возвращает или задает высоту 3‑D диаграммы в процентах от ширины диаграммы (от 5 до 500 процентов). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Указывает, скрывать ли кнопки полей сводной диаграммы только когда диаграмма является PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Указывает, является ли диаграмма 3‑D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Получает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Получает легенду диаграммы. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Получает линию. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Получает и задает имя диаграммы. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Получает коллекцию [`SeriesCollection`](../seriescollection/), представляющую серии данных в диаграмме. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Представляет описание настройки страницы в этой диаграмме. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Возвращает или задает перспективу трехмерного просмотра диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes равно True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Указывает элементы управления сводной таблицей, отображаемые на диаграмме |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Представляет способ привязки диаграммы к расположенным под ней ячейкам. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Получает область построения диаграммы, включающую подписи делений осей. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Получает и задает, строить ли по строкам или столбцам. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Получает и задает способ построения пустых ячеек. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Указывает, отображаются ли только видимые ячейки построения. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Указывает, отображаются ли только видимые ячейки построения. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Получает и задает размер печатной диаграммы. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | Истина, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Представляет вращение 3‑D представления диаграммы (вращение области построения вокруг оси z в градусах). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Получает вторую ось X диаграммы. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Получает вторую ось Y диаграммы. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Получает ось серии диаграммы. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Возвращает все графические фигуры в этой диаграмме. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Получает или задает значение, указывающее, отображает ли диаграмма таблицу данных. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Получает или задает значение, указывающее, будет ли отображена легенда диаграммы. По умолчанию — истина. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Возвращает объект [`Walls`](./walls/), представляющий боковую стенку 3‑D диаграммы. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | Истина, если Microsoft Excel изменяет размер диаграммы, чтобы он соответствовал размеру окна листа диаграммы. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Получает и задает встроенный стиль. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Получает подзаголовок диаграммы. Применяется только к файлам ODS. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Получает заголовок диаграммы. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Получает или задает тип диаграммы. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Получает ось Y диаграммы. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Возвращает объект [`Walls`](./walls/), представляющий стены 3‑D диаграммы. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | Истина, если линии сетки рисуются в двумерном виде на 3‑D диаграмме. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Получает лист, содержащий эту диаграмму. |

## Методы

| Имя | Описание |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Вычисляет пользовательские позиции области построения и осей, если их позиции назначаются автоматически. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Вычисляет пользовательскую позицию области построения и осей, если их позиция назначена автоматически, с использованием параметров расчёта диаграммы. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Изменить тип диаграммы с помощью предустановленного шаблона. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Получает фактический размер диаграммы в пикселях. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Получает диапазон источника данных диаграммы. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Возвращает, какие оси существуют на диаграмме. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Возвращает, относится ли ячейка к диаграмме. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Определяет, изменился ли источник данных диаграммы. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Возвращает, относится ли ячейка к диаграмме. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Перемещает диаграмму в указанное место. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Обновляет данные диаграммы из сводной таблицы. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Указывает диапазон данных для диаграммы. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Переключает строки/столбцы. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Получает 32‑битный объект `Bitmap` диаграммы. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Получает 32‑битный объект `Bitmap` диаграммы. Атрибуты `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality игнорируются. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Создаёт изображение диаграммы и сохраняет его в поток в формате Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Создаёт изображение диаграммы и сохраняет его в файл в указанном формате. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Создаёт изображение диаграммы и сохраняет его в файл в указанном типе изображения. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Создаёт изображение диаграммы и сохраняет его в файл в формате Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Создаёт PDF диаграммы и сохраняет его в поток. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Сохраняет диаграмму в pdf‑файл. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Создаёт pdf диаграммы и сохраняет его в поток. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Сохраняет диаграмму в pdf‑файл. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Установить свойства диаграммы
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Настроить внешний вид диаграммы
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Настроить оси диаграммы
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Настроить легенду диаграммы
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Настройте область построения диаграммы
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Настройте область диаграммы
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Сохраните книгу
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


