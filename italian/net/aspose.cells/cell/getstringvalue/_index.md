---
title: "Cell.GetStringValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene il valore stringa mediante una strategia di formattazione specifica"
type: docs
url: /it/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Ottiene il valore stringa mediante una strategia di formattazione specifica.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | La strategia formattata. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta diversi tipi di dati nelle celle
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // Dimostra GetStringValue con diverse strategie di formattazione
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### Vedi anche

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


