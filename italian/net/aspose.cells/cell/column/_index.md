---
title: "Cell.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il numero della colonna basato su zero della cella"
type: docs
url: /it/net/aspose.cells/cell/column/
---
## Cell.Column property

Restituisce il numero della colonna (basato su zero) della cella.

```csharp
public int Column { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alle celle e dimostra la proprietà Column
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Imposta valori e stili
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Dimostra l'uso della proprietà Column
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Modifica la larghezza della colonna usando la proprietà Column
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Salva la cartella di lavoro
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


