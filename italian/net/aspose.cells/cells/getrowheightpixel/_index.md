---
title: "Cells.GetRowHeightPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'altezza di una riga specificata in unità di pixel"
type: docs
url: /it/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Restituisce l'altezza di una riga specificata in unità di pixel.

```csharp
public int GetRowHeightPixel(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Altezza della riga

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Istanzia un nuovo Workbook
            Workbook wb = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = wb.Worksheets[0];

            // Imposta l'altezza della riga 5 (in pixel)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Ottieni l'altezza della riga 5 (in pixel)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


