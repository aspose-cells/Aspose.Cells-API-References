---
title: "Series.IsVerticalValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Указывает, является ли источник данных вертикальным"
type: docs
url: /ru/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Указывает, является ли источник данных вертикальным.

```csharp
public bool IsVerticalValues { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте серию с вертикальными значениями
            chart.NSeries.Add("A1:B10", true);
            
            // Продемонстрировать свойство IsVerticalValues (только для чтения)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Чтобы изменить ориентацию, нам нужно воссоздать серию с другими параметрами
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


