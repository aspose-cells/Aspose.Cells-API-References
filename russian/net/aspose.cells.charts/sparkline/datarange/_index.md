---
title: "Sparkline.DataRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Sparkline. Представляет диапазон данных спарклайна"
type: docs
url: /ru/net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Представляет диапазон данных спарклайна.

```csharp
public string DataRange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyDataRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(7);
            sheet.Cells["A4"].PutValue(2);
            sheet.Cells["A5"].PutValue(9);

            // Добавить группу спарклайнов
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Получите доступ к первому спарклайну и отобразите его диапазон данных
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
        }
    }
}
```

### См. также

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


