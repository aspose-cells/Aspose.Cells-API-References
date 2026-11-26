---
title: "DataLabels.IsTextWrapped"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Получает или задает значение, указывающее, будет ли текст переноситься"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Получает или задает значение, указывающее, будет ли текст переноситься.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsTextWrappedDemo
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
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(65);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к меткам данных
            Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
            
            // Показать подписи данных
            labels.ShowValue = true;
            
            // Продемонстрировать свойство IsTextWrapped
            Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
            labels.IsTextWrapped = true;
            Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);

            // Сохраните книгу
            workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


