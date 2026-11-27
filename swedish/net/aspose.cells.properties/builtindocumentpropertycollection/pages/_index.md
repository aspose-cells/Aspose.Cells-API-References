---
title: "BuiltInDocumentPropertyCollection.Pages"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet sidor i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/pages/
---
## BuiltInDocumentPropertyCollection.Pages property

Representerar en uppskattning av antalet sidor i dokumentet.

```csharp
public int Pages { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ställ in Pages-egenskapen
            builtInProperties.Pages = 10;

            // Lägg till ett kalkylblad och lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page Count Demonstration");
            worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");

            // Spara arbetsboken
            workbook.Save("DocumentPagesDemo.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


