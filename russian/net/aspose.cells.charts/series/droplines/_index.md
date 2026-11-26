---
title: "Series.DropLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает объект Line, представляющий линии падения для серии на линейной диаграмме или диаграмме области. Применяется только к линейным диаграммам или диаграммам области"
type: docs
url: /ru/net/aspose.cells.charts/series/droplines/
---
## Series.DropLines property

Возвращает объект [`Line`](../../../aspose.cells.drawing/line/) объект, представляющий линии падения для серии на линейной диаграмме или диаграмме области. Применяется только к линейным диаграммам или диаграммам области.

```csharp
public Line DropLines { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyDropLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["B5"].PutValue(210);

            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(130);
            worksheet.Cells["C4"].PutValue(160);
            worksheet.Cells["C5"].PutValue(190);

            // Добавить линейную диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Включите линии падения для диаграммы
            chart.NSeries[0].HasDropLines = true;
            chart.NSeries[1].HasDropLines = true;

            // Получите доступ к линиям падения первой серии
            Line dropLines = chart.NSeries[0].DropLines;

            // Отобразите текущие свойства линий падения
            Console.WriteLine("Drop line color: " + dropLines.Color);
            Console.WriteLine("Drop line style: " + dropLines.Style);
            Console.WriteLine("Drop line weight: " + dropLines.Weight);

            // Измените свойства линий падения
            dropLines.Color = System.Drawing.Color.Red;
            dropLines.Style = LineType.Solid;
            dropLines.Weight = WeightType.MediumLine;
            dropLines.DashType = MsoLineDashStyle.Solid;
            dropLines.IsVisible = true;

            // Сохраните книгу
            workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


