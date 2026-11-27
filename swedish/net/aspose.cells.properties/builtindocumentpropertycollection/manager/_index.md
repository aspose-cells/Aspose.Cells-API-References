---
title: "BuiltInDocumentPropertyCollection.Manager"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger manager-egenskapen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Hämtar eller anger manager‑egenskapen.

```csharp
public string Manager { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange grundläggande dokumentegenskaper inklusive Manager
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
            builtInProperties.Company = "Aspose";

            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx");

            Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


