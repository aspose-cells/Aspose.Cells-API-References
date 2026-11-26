---
title: "DataLabels.IsAutoText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Указывает, что текст генерируется автоматически"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Указывает, что текст сгенерирован автоматически.

```csharp
public override bool IsAutoText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsAutoTextDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить подписи данных
            foreach (Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
                
                // Продемонстрировать свойство IsAutoText
                foreach (ChartPoint point in series.Points)
                {
                    Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
                    point.DataLabels.IsAutoText = false;
                    point.DataLabels.Text = "Custom " + point.YValue;
                    Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
                    Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
                }
            }
            
            // Сохраните книгу
            workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


