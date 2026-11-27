---
title: "BuiltInDocumentPropertyCollection.DocumentVersion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Representerar filens version"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

Representerar filens version.

```csharp
public string DocumentVersion { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in dokumentversionsegenskapen
            workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
            
            // Visa dokumentversionen
            Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
            
            // Spara arbetsboken
            workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


