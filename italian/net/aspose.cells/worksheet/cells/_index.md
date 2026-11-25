---
title: "Worksheet.Cells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la collezione Cells"
type: docs
url: /it/net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Ottiene la collezione [`Cells`](../../cells/) nel foglio di lavoro.

```csharp
public Cells Cells { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di celle
            Cells cells = worksheet.Cells;
            
            // Imposta valori nelle celle
            cells["A1"].PutValue("Item");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);
            
            // Imposta la formula per calcolare il totale
            cells["A4"].PutValue("Total:");
            cells["B4"].Formula = "=SUM(B2:B3)";
            
            // Calcola le formule
            workbook.CalculateFormula();
            
            // Visualizza i valori delle celle
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);
            Console.WriteLine("B2: " + cells["B2"].StringValue);
            Console.WriteLine("A3: " + cells["A3"].StringValue);
            Console.WriteLine("B3: " + cells["B3"].StringValue);
            Console.WriteLine("A4: " + cells["A4"].StringValue);
            Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
            
            // Salva cartella di lavoro
            workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


