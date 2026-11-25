---
title: "Cells.StandardHeightPixels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Restituisce o imposta l'altezza predefinita della riga in questo foglio di lavoro nell'unità di pixel"
type: docs
url: /it/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di pixel.

```csharp
public int StandardHeightPixels { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta alcuni dati nelle celle
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Ottieni l'altezza standard in pixel
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Visualizza le altezze delle righe (dovrebbe corrispondere all'altezza standard)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Modifica l'altezza standard e verifica
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Verifica che tutte le righe ora abbiano la nuova altezza
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


