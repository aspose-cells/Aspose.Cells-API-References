---
title: "Chart.PlotBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает и задает, отображать ли по строке или по столбцу"
type: docs
url: /ru/net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Получает и задает, строить ли по строкам или столбцам.

```csharp
public PlotDataByType PlotBy { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotByDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.SetChartDataRange("A1:C4", true);

            // Продемонстрировать свойство PlotBy
            Console.WriteLine("Default PlotBy: " + chart.PlotBy);
            
            // Создать новую диаграмму с другой настройкой plot by
            int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
            Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
            newChart.SetChartDataRange("A1:C4", false); // Plot by row
            Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);

            // Сохраните книгу
            workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


