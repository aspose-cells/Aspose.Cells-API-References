---
title: "ConditionalFormattingResult.ConditionalStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingResult-egenskap. Hämtar den villkorliga resultatstilen"
type: docs
url: /sv/net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Hämtar den villkorsstyrda resultatstilen.

```csharp
public Style ConditionalStyle { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            
            // Skapa villkor och ange stil
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            fc.Style = style;

            // Hämta cell med villkorlig formatering
            Cell cell = worksheet.Cells["A3"];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            
            // Skriv ut färgen för att demonstrera egenskapen
            Console.WriteLine("Conditional Style Font Color: " + conditionalStyle.Font.Color);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


