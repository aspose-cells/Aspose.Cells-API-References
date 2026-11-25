---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la raccolta HorizontalPageBreakCollection"
type: docs
url: /it/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Ottiene la raccolta [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/).

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi interruzioni di pagina orizzontali in modi diversi
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // Rimuovi la prima interruzione di pagina
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Salva i risultati
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


