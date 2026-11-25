---
title: "Range.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene la larghezza di un intervallo in punti"
type: docs
url: /it/net/aspose.cells/range/height/
---
## Range.Height property

Ottiene la larghezza di un intervallo in punti.

```csharp
public double Height { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le altezze delle righe per la dimostrazione
            worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
            worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
            worksheet.Cells.SetRowHeight(3, 25.0); // Row 4

            // Crea un intervallo che copre le righe 2-4 (B2:C4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Dimostra la proprietà Height
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Calculated Height (sum of row heights): " + 
                (worksheet.Cells.GetRowHeight(1) + 
                 worksheet.Cells.GetRowHeight(2) + 
                 worksheet.Cells.GetRowHeight(3)));
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


