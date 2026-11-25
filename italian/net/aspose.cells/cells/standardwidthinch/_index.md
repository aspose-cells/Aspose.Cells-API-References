---
title: "Cells.StandardWidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro in unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pollici.

```csharp
public double StandardWidthInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la larghezza standard della colonna in pollici
            worksheet.Cells.StandardWidthInch = 1.5;

            // Imposta la larghezza specifica della colonna in pollici a scopo dimostrativo
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Salva la cartella di lavoro
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


