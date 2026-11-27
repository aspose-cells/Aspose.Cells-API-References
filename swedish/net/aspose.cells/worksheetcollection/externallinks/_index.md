---
title: "WorksheetCollection.ExternalLinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Representerar externa länkar i en arbetsbok"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Representerar externa länkar i en arbetsbok.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok med extern länk
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Skapa en målarbetsbok
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Ange datakälla för extern länk
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Spara arbetsboken
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Rensa upp
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


