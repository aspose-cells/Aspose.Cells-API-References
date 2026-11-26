---
title: "Series.DataLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет объект DataLabels для указанного ASeries"
type: docs
url: /ru/net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Представляет объект DataLabels для указанного ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Products");
            dataSheet.Cells["B1"].PutValue("Users");
            dataSheet.Cells["A2"].PutValue("Aspose.Cells");
            dataSheet.Cells["B2"].PutValue(10000);
            dataSheet.Cells["A3"].PutValue("Aspose.Slides");
            dataSheet.Cells["B3"].PutValue(8000);
            dataSheet.Cells["A4"].PutValue("Aspose.Words");
            dataSheet.Cells["B4"].PutValue(12000);

            // Добавьте лист диаграммы и создайте круговую диаграмму
            Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
            Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

            // Добавить данные серии и настроить подписи данных
            Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
            series.XValues = "=Sheet1!$A$2:$A$4";
            
            // Настроить свойства DataLabels
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCategoryName = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.LinkedSource = null; // Explicitly set to null

            // Сохраните книгу
            workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


