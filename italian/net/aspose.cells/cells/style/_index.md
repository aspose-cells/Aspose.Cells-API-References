---
title: "Cells.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene e imposta lo stile predefinito del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/style/
---
## Cells.Style property

Ottiene e imposta lo stile predefinito del foglio di lavoro.

```csharp
public Style Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta un valore nella cella A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Ottieni lo stile predefinito e modifica il suo formato
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Applica lo stile modificato alla cella
            cell.SetStyle(style);

            // Visualizza il valore stringa formattato
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


