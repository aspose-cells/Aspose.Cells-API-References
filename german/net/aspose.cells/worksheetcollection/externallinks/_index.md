---
title: "WorksheetCollection.ExternalLinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Stellt externe Links in einer Arbeitsmappe dar"
type: docs
url: /de/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Stellt externe Links in einer Arbeitsmappe dar.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Erstelle eine Quellarbeitsmappe mit externem Link
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Erstelle eine Ziel-Arbeitsmappe.
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Setze die Datenquelle des externen Links
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Speichere die Arbeitsmappe
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Aufräumen
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Siehe auch

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


