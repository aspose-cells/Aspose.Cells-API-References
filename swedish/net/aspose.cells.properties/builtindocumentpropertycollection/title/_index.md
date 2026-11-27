---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger dokumentets titel"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Hämtar eller anger titeln på dokumentet.

```csharp
public string Title { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in Title‑egenskapen
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Visa Title‑egenskapen
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


