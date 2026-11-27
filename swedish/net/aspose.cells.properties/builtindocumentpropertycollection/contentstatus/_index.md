---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger dokumentets innehållsstatus"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Hämtar eller anger innehållsstatus för dokumentet.

```csharp
public string ContentStatus { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in inbyggda dokumentegenskaper inklusive ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Spara arbetsboken
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // Visa ContentStatus‑egenskapen
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


