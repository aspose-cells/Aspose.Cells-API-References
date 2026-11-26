---
title: "LegendEntry.IsTextNoFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LegendEntry. Получает или задает отсутствие заливки текста"
type: docs
url: /ru/net/aspose.cells.charts/legendentry/istextnofill/
---
## LegendEntry.IsTextNoFill property

Получает или задает отсутствие заливки текста.

```csharp
public bool IsTextNoFill { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsTextNoFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Получить доступ к записи легенды и установить IsTextNoFill
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.IsTextNoFill = true; // Text will have no fill
            
            // Сохраните книгу
            workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


