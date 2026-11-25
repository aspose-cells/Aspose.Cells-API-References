---
title: "Cells.SetRowHeightPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta l'altezza della riga in unità di pixel"
type: docs
url: /it/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Imposta l'altezza della riga in unità di pixel.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| pixel | Int32 | Numero di pixel. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta l'altezza della prima riga a 50 pixel
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Imposta l'altezza della seconda riga a 100 pixel
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Salva la cartella di lavoro
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


