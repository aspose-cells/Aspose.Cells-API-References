---
title: "DataLabels.BackgroundMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Получает и задает режим отображения фона"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Получает и задает режим отображения фона

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(5);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Получить подписи данных
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Продемонстрировать свойство BackgroundMode
            dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
            Console.WriteLine("BackgroundMode set to Automatic");

            // Сохраните книгу
            workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


