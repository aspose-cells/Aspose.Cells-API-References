---
title: "BuiltInDocumentPropertyCollection.NameOfApplication"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger namnet på applikationen"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Hämtar eller anger namnet på applikationen.

```csharp
public string NameOfApplication { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in NameOfApplication-egenskapen
            workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
            
            // Visa NameOfApplication-egenskapen
            Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
            
            // Spara arbetsboken
            workbook.Save("output.ods");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


