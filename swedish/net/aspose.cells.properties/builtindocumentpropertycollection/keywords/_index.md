---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger dokumentets nyckelord"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Hämtar eller anger dokumentets nyckelord.

```csharp
public string Keywords { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in Keywords-egenskapen
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Spara arbetsboken
            workbook.Save("output_keywords.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera Keywords-egenskapen
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Visa egenskapen Keywords
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


