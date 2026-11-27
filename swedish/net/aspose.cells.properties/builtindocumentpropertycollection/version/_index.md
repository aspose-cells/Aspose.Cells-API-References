---
title: "BuiltInDocumentPropertyCollection.Version"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar versionsnumret för programmet som skapade dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Representerar versionsnumret för programmet som skapade dokumentet.

```csharp
public string Version { get; set; }
```

### Anmärkningar

Dess format är "00.0000", till exempel: 12.0000

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in några dokumentegenskaper
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Åtkomst och visa Version-egenskapen
            string version = workbook.BuiltInDocumentProperties.Version;
            Console.WriteLine("Document Version: " + version);
            
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


