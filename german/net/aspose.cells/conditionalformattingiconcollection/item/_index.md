---
title: "ConditionalFormattingIconCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIconCollection‑Eigenschaft. Gibt das ConditionalFormattingIcon‑Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Ruft das ConditionalFormattingIcon‑Element am angegebenen Index ab.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

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

            // Demonstriere die Verwendung der Item-Eigenschaft
            ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
            icon.Type = IconSetType.Arrows3;
            icon.Index = 0;

            workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


