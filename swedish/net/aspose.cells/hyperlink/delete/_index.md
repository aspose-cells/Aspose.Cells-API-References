---
title: "Hyperlink.Delete"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑metod. Tar bort denna hyperlänk"
type: docs
url: /sv/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Tar bort denna hyperlänk

```csharp
public void Delete()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några hyperlänkar för att demonstrera borttagning
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // Ta bort alla hyperlänkar
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Se även

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


