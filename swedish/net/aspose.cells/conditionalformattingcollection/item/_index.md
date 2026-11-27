---
title: "ConditionalFormattingCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingCollection-egenskapen. Hämtar FormatConditions-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Hämtar FormatConditions-elementet på det angivna indexet.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Lägg till villkorsstyrd formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            // Lägg till formatvillkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Kom åt och demonstrera användning av Item-egenskapen
            FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
            Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
            Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


