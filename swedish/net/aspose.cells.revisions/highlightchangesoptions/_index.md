---
title: "Klass HighlightChangesOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.HighlightChangesOptions-klass. Representerar alternativ för att markera revisioner eller ändringar i delade Excel-filer"
type: docs
url: /sv/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Representerar alternativ för att markera revisioner eller ändringar i delade Excel‑filer.

```csharp
public class HighlightChangesOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Representerar alternativ för att markera revisioner eller ändringar i delade Excel‑filer. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Instansiera ett Workbook-objekt
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Hämta revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Ställ in antalet dagar för att bevara historiken
            revisionLogs.DaysPreservingHistory = 30;

            // Skapa HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Markera ändringar
            revisionLogs.HighlightChanges(options);

            // Spara arbetsboken med markerade ändringar
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


