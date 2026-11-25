---
title: "Range.Left"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce la distanza in punti dal bordo sinistro della colonna A al bordo sinistro dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/left/
---
## Range.Left property

Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo.

```csharp
public double Left { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo da B2 a C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Dimostra l'uso della proprietà Left
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Calcola i valori attesi in base al caso di test
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


