---
title: "Range.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene la larghezza di un intervallo in punti"
type: docs
url: /it/net/aspose.cells/range/width/
---
## Range.Width property

Ottiene la larghezza di un intervallo in punti.

```csharp
public double Width { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le larghezze delle colonne per dimostrare la proprietà Width
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Visualizza la larghezza dell'intervallo (somma delle larghezze delle colonne nell'intervallo)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Visualizza le proprietà individuali per verifica
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


