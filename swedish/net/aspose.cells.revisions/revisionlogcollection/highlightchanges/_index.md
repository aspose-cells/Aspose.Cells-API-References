---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionLogCollection-metod. Markerar ändringar i delad arbetsbok"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Markerar ändringar i delad arbetsbok.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | HighlightChangesOptions | Ställ in alternativen för att filtrera vilka ändringar som ska spåras. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och revisioner
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Markera ändringar med alternativ
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


