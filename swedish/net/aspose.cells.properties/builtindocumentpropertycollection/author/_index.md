---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger namnet på dokumentets författare"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Hämtar eller anger namnet på dokumentets författare.

```csharp
public string Author { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in författaregenskapen
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Visa författaregenskapen
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


