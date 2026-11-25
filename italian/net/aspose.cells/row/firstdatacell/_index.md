---
title: "Row.FirstDataCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Ottiene la prima cella non vuota nella riga"
type: docs
url: /it/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Ottiene la prima cella non vuota nella riga.

```csharp
public Cell FirstDataCell { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Inserisci valori in celle diverse
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Ottieni la prima cella dati nella riga 1 (indice 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Ottieni la prima cella dati nella riga 2 (indice 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


