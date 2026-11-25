---
title: "Cells.StandardHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro in unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di pollici.

```csharp
public double StandardHeightInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni l'altezza standard in pollici
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Imposta una nuova altezza standard (1 pollice)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


