---
title: "Cells.StandardWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro in unità di caratteri"
type: docs
url: /it/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di caratteri.

```csharp
public double StandardWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la larghezza standard per le colonne
            cells.StandardWidth = 18.25;

            // Visualizza la larghezza standard e la larghezza effettiva della prima colonna
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Verifica che la larghezza standard sia applicata (approssimativamente)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


