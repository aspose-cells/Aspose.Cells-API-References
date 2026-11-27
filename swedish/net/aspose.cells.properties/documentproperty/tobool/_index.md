---
title: "DocumentProperty.ToBool"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentProperty metod. Returnerar egenskapsvärdet som bool"
type: docs
url: /sv/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Returnerar egenskapsvärdet som bool.

```csharp
public bool ToBool()
```

### Anmärkningar

Kastar ett undantag om egenskapstypen inte är PropertyType.Boolean.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till en boolesk anpassad dokumentegenskap
            customProperties.Add("IsApproved", true);
            
            // Hämta egenskapen och konvertera till bool med ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Se även

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


