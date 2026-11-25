---
title: "Cells.StandardHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro in unità di punti"
type: docs
url: /it/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di punti.

```csharp
public double StandardHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni e visualizza l'altezza standard
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Imposta una nuova altezza standard
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Salva la cartella di lavoro
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


