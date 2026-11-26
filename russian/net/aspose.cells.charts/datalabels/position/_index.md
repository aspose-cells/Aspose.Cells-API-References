---
title: "DataLabels.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DataLabels property. Представляет позицию подписи данных"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Представляет позицию метки данных.

```csharp
public LabelPositionType Position { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить подписи данных
            chart.NSeries[0].DataLabels.ShowValue = true;
            
            // Установить позицию подписи данных
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

            // Сохраните книгу
            workbook.Save("DataLabelsPositionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


