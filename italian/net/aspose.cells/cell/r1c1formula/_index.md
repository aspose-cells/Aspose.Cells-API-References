---
title: "Cell.R1C1Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene o imposta una formula R1C1 della cella"
type: docs
url: /it/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Ottiene o imposta una formula R1C1 del [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta valore A1
            worksheet.Cells["A1"].PutValue(10);
            
            // Imposta valore B1
            worksheet.Cells["B1"].PutValue(20);
            
            // Imposta formula C1 in notazione A1
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Ottieni e visualizza la formula R1C1
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Imposta formula D1 in notazione R1C5
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Ottieni e visualizza la formula A1
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Salva la cartella di lavoro
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


