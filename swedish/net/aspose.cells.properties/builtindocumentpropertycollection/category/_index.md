---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection property. Hämtar eller anger dokumentets kategori"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Hämtar eller anger kategorin för dokumentet.

```csharp
public string Category { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            var workbook = new Workbook();
            
            // Ställ in inbyggda dokumentegenskaper
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // Spara till minnesström
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // Läs in arbetsboken igen från strömmen
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // Visa egenskaperna
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


