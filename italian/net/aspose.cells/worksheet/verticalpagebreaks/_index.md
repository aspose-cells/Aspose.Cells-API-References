---
title: "Worksheet.VerticalPageBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Restituisce la collezione VerticalPageBreakCollection"
type: docs
url: /it/net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Restituisce la collezione [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/).

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVerticalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Aggiungi diversi tipi di interruzioni di pagina verticali
            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            // Rimuovi un'interruzione
            verticalPageBreaks.RemoveAt(1);

            // Stampa le informazioni sull'interruzione
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


