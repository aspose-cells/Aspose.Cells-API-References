---
title: "Cell.FloatValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce il valore float contenuto nella cella."
type: docs
url: /it/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Restituisce il valore float contenuto nella cella.

```csharp
public float FloatValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il valore numerico direttamente
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // Imposta una formula che restituisce un float
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // Dimostra FloatValue con una formula condivisa
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


