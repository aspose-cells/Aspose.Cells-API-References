---
title: "BuiltInDocumentPropertyCollection.ContentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection property. Hämtar eller anger dokumentets innehållstyp"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

Hämtar eller anger innehållstypen för dokumentet.

```csharp
public string ContentType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ange ContentType‑egenskapen
            workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";

            // Visa ContentType‑egenskapen
            Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);

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


