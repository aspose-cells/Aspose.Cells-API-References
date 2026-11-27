---
title: "Workbook.AcceptAllRevisions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Accepterar alla spårade ändringar i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accepterar alla spårade ändringar i arbetsboken.

```csharp
public void AcceptAllRevisions()
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med revisioner
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några revisioner (spåra ändringar måste vara aktiverat i Excel först)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Spara med revisioner
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Öppna arbetsboken igen
            workbook = new Workbook(sourcePath);
            
            // Kontrollera om den har revisioner och acceptera dem
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Spara utan revisioner
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


