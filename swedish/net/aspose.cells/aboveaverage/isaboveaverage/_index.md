---
title: "AboveAverage.IsAboveAverage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AboveAverage egenskap. Hämta eller ange flaggan som indikerar om regeln är en över genomsnittlig regel. true indikerar över genomsnittet. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Hämta eller ange flaggan som indikerar om regeln är en \"above average\"-regel. 'true' betyder 'above average'. Standardvärdet är true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera den villkorliga formateringen
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Lägg till en villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ange området för villkorsformatering
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Lägg till ett AboveAverage‑villkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Konfigurera AboveAverage‑egenskaperna
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Spara Excel-filen
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Se även

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


