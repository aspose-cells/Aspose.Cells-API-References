---
title: "Cells.StandardWidthPixels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro in unità di pixel"
type: docs
url: /it/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pixel.

```csharp
public int StandardWidthPixels { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta e ottieni la larghezza standard in pixel
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Imposta e ottieni la larghezza standard in caratteri
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Imposta e ottieni l'altezza standard in punti
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


