---
title: "ConditionalFormattingIconCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIconCollection-egenskap. Hämtar ConditionalFormattingIcon-elementet på det angivna indexet."
type: docs
url: /sv/net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Hämtar ConditionalFormattingIcon-elementet på det angivna indexet.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;
            int index = cformattings.Add();
            FormatConditionCollection fcs = cformattings[index];

            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 });
            fcs.AddArea(new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 });

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Demonstrera användning av Item-egenskapen
            ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
            icon.Type = IconSetType.Arrows3;
            icon.Index = 0;

            workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


