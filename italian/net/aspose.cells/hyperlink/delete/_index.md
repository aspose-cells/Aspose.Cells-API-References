---
title: "Hyperlink.Delete"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Hyperlink. Elimina questo hyperlink"
type: docs
url: /it/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Elimina questo collegamento ipertestuale

```csharp
public void Delete()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni hyperlink per dimostrare l'eliminazione
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // Elimina tutti gli hyperlink
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


