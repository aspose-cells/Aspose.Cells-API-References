---
title: "Workbook.HasRevisions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar om arbetsboken har några spårade ändringar"
type: docs
url: /sv/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Hämtar om arbetsboken har några spårade ändringar

```csharp
public bool HasRevisions { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med revisioner
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gör en ändring som skapar en revision
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Kontrollera om arbetsboken har revisioner
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Godkänn alla revisioner (om några)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Kontrollera igen efter att ha accepterat revideringar
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


