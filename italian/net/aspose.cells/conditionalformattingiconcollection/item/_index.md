---
title: "ConditionalFormattingIconCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConditionalFormattingIconCollection proprietà. Ottiene l'elemento ConditionalFormattingIcon all'indice specificato"
type: docs
url: /it/net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Recupera l'elemento ConditionalFormattingIcon all'indice specificato.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

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

            // Dimostra l'uso della proprietà Item
            ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
            icon.Type = IconSetType.Arrows3;
            icon.Index = 0;

            workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


