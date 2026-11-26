---
title: "Класс Series"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Series. Инкапсулирует объект, представляющий одну серию данных в диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/series/
---
## Series class

Инкапсулирует объект, представляющий отдельную серию данных в диаграмме.

```csharp
public class Series
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Представляет область фона объекта Series. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Получает или задает тип 3D‑формы, используемой в 3‑D столбчатой или колонковой диаграмме. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Представляет границу объекта Series. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Получает или задает коэффициент масштабирования пузырей в указанной группе диаграмм. Это может быть целое значение от 0 (ноль) до 300, соответствующее проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Получает или задает значения размеров пузырей серии диаграммы. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Получает кэшированные значения категорий для серии |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Получает кэшированные значения для серии |
| [CategoryValues](../../aspose.cells.charts/series/categoryvalues/) { get; } | Получает фактические значения категорий, используемые для построения каждой точки этой серии в диаграмме. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Получает количество значений данных. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Представляет объект DataLabels для указанного ASeries. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Получает имя серии, отображаемое на графике диаграммы. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Возвращает или задает размер отверстия в группе кольцевой диаграммы. Размер отверстия выражается в процентах от размера диаграммы, от 10 до 90 процентов. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Возвращает объект [`DropBars`](../dropbars/), представляющий нижние бары на линейной диаграмме. Применяется только к линейным диаграммам. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Возвращает объект [`Line`](../../aspose.cells.drawing/line/), представляющий линии падения для серии на линейной или областной диаграмме. Применяется только к линейным и областным диаграммам. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | Расстояние открытого сектора круговой диаграммы от её центра выражается в процентах от диаметра диаграммы. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, значения от 0 до 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Возвращает или задает пространство между кластерами столбцов или колонок в процентах от их ширины. Значение этого свойства должно быть от 0 до 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | Истина, если у серии трехмерный вид. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | Истина, если у диаграммы есть линии падения. Применяется только к линейным или областным диаграммам. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | Истина, если у линейной диаграммы есть линии максимум‑минимум. Применяется только к линейным диаграммам. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | Истина, если у серии есть линии‑выноски. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | Истина, если у радиальной диаграммы есть подписи оси категорий. Применяется только к радиальным диаграммам. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | Истина, если у сложенной столбчатой или гистограммы есть линии серии, или если у диаграммы «Круг в круге» или «Бар в круге» есть соединительные линии между двумя секциями. Применяется только к сложенным столбчатым диаграммам, гистограммам, диаграммам «Круг в круге» и «Бар в круге». |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | Истина, если у линейной диаграммы есть бары вверх и вниз. Применяется только к линейным диаграммам. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Возвращает объект HiLoLines, представляющий линии максимум‑минимум для серии на линейной диаграмме. Применяется только к линейным диаграммам. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Указывает, является ли значение порога автоматическим. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Представляет, варьируется ли цвет точек. Диаграмма должна содержать только одну серию или быть круговой диаграммой. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Указывает, выбрана ли серия или отфильтрована. Истина означает, что эта серия отфильтрована и не будет отображаться на диаграмме. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Указывает, является ли источник данных вертикальным. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Представляет свойства макета. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Представляет линии‑выноски на диаграмме. Линии‑выноски соединяют подписи данных с точками данных. Этот объект не является коллекцией; нет объекта, представляющего отдельную линию‑выноску. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Получает элемент легенды, соответствующий этой серии. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Получает [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Получает или задает имя серии данных. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Указывает, как позиционируются бары и столбцы. Может принимать значение от -100 до 100. Применяется только к 2‑D барным и 2‑D столбчатым диаграммам. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Указывает, построен ли этот ряд на второй оси значений. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Получает коллекцию точек в ряду диаграммы. |
| [PointValues](../../aspose.cells.charts/series/pointvalues/) { get; } | Получает фактические значения, используемые для построения каждой точки этого ряда на диаграмме. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Возвращает или задает размер вторичной части либо диаграммы «круг в круге», либо «полоска в круге», в процентах от размера основного круга. Может принимать значение от 5 до 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Возвращает объект SeriesLines, представляющий линии рядов для сложенной гистограммы или сложенной столбчатой диаграммы. Применяется только к сложенным гистограммам и столбчатым диаграммам. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | Истина, если у ряда есть тень. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Получает объект [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/), содержащий визуальные свойства формы ряда. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | Истина, если для группы диаграммы отображаются отрицательные пузыри. Действительно только для пузырьковых диаграмм. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Получает или задает, что представляет размер пузыря на пузырьковой диаграмме. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Представляет сглаживание кривой. Истина, если сглаживание включено для линейной диаграммы или диаграммы разброса. Применяется только к линейным диаграммам и диаграммам разброса с линиями. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Возвращает или задает значение, определяющее, какие точки данных находятся во второй части (круге или полосе) диаграммы «круг в круге» или «полоска в круге». |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Возвращает или задает значение, которое будет использоваться для определения, какие точки данных находятся во второй части (круге или полосе) диаграммы «круг в круге» или «полоска в круге». |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Возвращает все линии тренда этого ряда. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Получает или задает тип ряда данных. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Возвращает объект DropBars, представляющий верхние бары на линейной диаграмме. Применяется только к линейным диаграммам. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Представляет значения Y этого ряда диаграммы. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Представляет код формата списка чисел Values. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Представляет ошибочную полосу по направлению X ряда. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Представляет значения X этого ряда диаграммы. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Представляет код формата списка чисел X Values. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Представляет ошибочную полосу по направлению Y ряда. |

## Методы

| Имя | Описание |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Перемещает ряд вверх или вниз. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesDemo
    {
        public static void SeriesExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Установка источника данных для категориальных данных NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Доступ к ряду
            Series series = chart.NSeries[seriesIndex];

            // Установка значений серии
            series.Values = "=B1:B4";
            // Изменение типа диаграммы ряда
            series.Type = ChartType.Line;
            // Настройка свойств маркера
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Настройка дополнительных свойств
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Сохранение файла Excel
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


