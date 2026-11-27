---
title: "AboveAverage.StdDev"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AboveAverage-egenskap. Hämtar eller anger antalet standardavvikelser som ska inkluderas ovanför eller under medelvärdet i den villkorliga formateringsregeln. Inmatningsvärdet måste ligga mellan 0 och 3, inklusive 0 och 3. Att sätta detta värde till 0 betyder att stdDev inte är angivet. Standardvärdet är 0"
type: docs
url: /sv/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Hämta eller ange antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. Inmatningsvärdet måste vara mellan 0 och 3 (inklusive 0 och 3). Att sätta värdet till 0 betyder att stdDev inte är angivet. Standardvärdet är 0.

```csharp
public int StdDev { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Fyll i exempeldata
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Se även

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


