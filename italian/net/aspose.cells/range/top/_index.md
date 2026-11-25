---
title: "Range.Top"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene la distanza in punti dal bordo superiore della riga 1 al bordo superiore dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/top/
---
## Range.Top property

Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo.

```csharp
public double Top { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo e imposta alcuni valori
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Dimostra l'uso della proprietà Top
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


