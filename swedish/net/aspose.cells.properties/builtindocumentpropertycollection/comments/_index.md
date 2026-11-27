---
title: "BuiltInDocumentPropertyCollection.Comments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller sätter dokumentkommentarerna"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Hämtar eller anger dokumentkommentarerna.

```csharp
public string Comments { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Ställ in egenskapen Comments
            properties.Comments = "This is a sample comment for demonstration.";
            
            // Visa egenskapen Comments
            Console.WriteLine("Document Comments: " + properties.Comments);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


