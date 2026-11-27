---
title: "AboveAverage.IsEqualAverage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AboveAverage-egenskap. Hämtar eller anger flaggan som indikerar om kriterierna aboveAverage och belowAverage är inklusiva för själva medelvärdet eller exkluderar det värdet. true betyder att medelvärdet inkluderas i kriterierna. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Hämta eller ange flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. 'true' betyder att genomsnittsvärdet inkluderas i kriterierna. Standardvärdet är false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
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
            fc.Style.BackgroundColor = Color.LightBlue;

            // Demonstrera IsEqualAverage-egenskapen
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Fyll i exempeldata
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### Se även

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


