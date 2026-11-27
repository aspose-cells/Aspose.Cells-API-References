---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Anger visningsläget för dokumentets miniatyrbild"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Anger visningsläget för dokumentets miniatyrbild.

```csharp
public bool ScaleCrop { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Ställ in ScaleCrop‑egenskapen
            properties.ScaleCrop = true;
            
            // Visa ScaleCrop‑egenskapens värde
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
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


