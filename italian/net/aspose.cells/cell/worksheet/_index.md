---
title: "Cell.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il foglio di lavoro genitore"
type: docs
url: /it/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Ottiene il foglio di lavoro genitore.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Accedi a una cella e dimostra la proprietà Worksheet
            Cell cell = worksheet.Cells["A3"];
            
            // Visualizza le informazioni del foglio di lavoro tramite la proprietà Worksheet della cella
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Aggiungi un altro foglio di lavoro e dimostra il riferimento incrociato tra fogli
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Accedi alla cella in Sheet2 e mostra il suo foglio di lavoro
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


