---
title: "DataLabels.ShowCellRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Указывает, следует ли показывать диапазон ячеек в качестве подписей данных"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Указывает, следует ли отображать диапазон ячеек в качестве меток данных.

```csharp
public bool ShowCellRange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCellRangeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Настроить подписи данных с помощью ShowCellRange
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Сохраните книгу
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


