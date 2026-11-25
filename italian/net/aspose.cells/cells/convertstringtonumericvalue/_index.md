---
title: "Cells.ConvertStringToNumericValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Converte tutti i dati stringa nel foglio di lavoro in valori numerici, se possibile"
type: docs
url: /it/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Converte tutti i dati stringa nel foglio di lavoro in valore numerico, se possibile.

```csharp
public void ConvertStringToNumericValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Inserisci valori stringa che possono essere convertiti in valori numerici
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Converti i valori stringa in numerici dove possibile
            cells.ConvertStringToNumericValue();

            // Visualizza i valori convertiti
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


