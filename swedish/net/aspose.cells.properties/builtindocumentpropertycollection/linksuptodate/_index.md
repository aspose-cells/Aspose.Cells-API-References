---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Anger om hyperlänkar i ett dokument är uppdaterade"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Indikerar om hyperlänkar i ett dokument är aktuella.

```csharp
public bool LinksUpToDate { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till den inbyggda samlingen av dokumentegenskaper
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange LinksUpToDate-egenskapen för att indikera om hyperlänkar är aktuella
            builtInProperties.LinksUpToDate = true;

            // Lägg till en enkel hyperlänk för att demonstrera egenskapen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Spara arbetsboken
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


