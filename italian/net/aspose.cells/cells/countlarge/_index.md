---
title: "Cells.CountLarge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene il conteggio totale degli oggetti Cell istanziati"
type: docs
url: /it/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Ottiene il conteggio totale degli oggetti Cell istanziati.

```csharp
public long CountLarge { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Dimostra la proprietà CountLarge
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Mostra le dimensioni della carta per la dimostrazione
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


