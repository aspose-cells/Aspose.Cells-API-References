---
title: "Chart.PlotEmptyCellsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает и задаёт способ построения пустых ячеек"
type: docs
url: /ru/net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Получает и задает способ построения пустых ячеек.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные с некоторыми пустыми ячейками
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            // B3 оставлена пустой
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство PlotEmptyCellsType
            chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
            Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);

            // Сохраните книгу
            workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


