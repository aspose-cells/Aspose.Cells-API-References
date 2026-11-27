---
title: "BuiltInDocumentPropertyCollection.Words"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar en uppskattning av antalet ord i dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/words/
---
## BuiltInDocumentPropertyCollection.Words property

Representerar en uppskattning av antalet ord i dokumentet.

```csharp
public int Words { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till de inbyggda dokumentegenskaperna
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Ange Words-egenskapen
            builtInProperties.Words = 250;

            // Lägg till lite innehåll i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample document");
            worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
            worksheet.Cells["A3"].PutValue("Total words will be set to 250");

            // Spara arbetsboken
            workbook.Save("DocumentWithWordsProperty.xlsx");

            Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


