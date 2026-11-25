---
title: "FindOptions.SetRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FindOptions. Imposta l'intervallo di ricerca"
type: docs
url: /it/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Imposta l'intervallo cercato.

```csharp
public void SetRange(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | l'intervallo di ricerca. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // Crea FindOptions e imposta l'intervallo di ricerca
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Cerca all'interno dell'intervallo specificato
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


