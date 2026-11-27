---
title: "ConditionalFormattingResult.ConditionalFormattingIcon"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingResult-egenskap. Hämtar bilden av ikonsättet"
type: docs
url: /sv/net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Hämtar bilden av ikonsatsen.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och villkorsstyrd formatering
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till villkorsformatering med ikonset
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Beräkna formler och hämta resultatet av villkorsformatering
            workbook.CalculateFormula();
            ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();

            // Visa ConditionalFormattingIcon-egenskapen
            if (result != null && result.ConditionalFormattingIcon != null)
            {
                Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
                Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
            }
        }
    }
}
```

### Se även

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


