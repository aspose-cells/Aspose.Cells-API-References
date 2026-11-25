---
title: "CellValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellValue. Ottiene o imposta il tipo del valore della cella"
type: docs
url: /it/net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Ottiene o imposta il tipo di valore della cella.

```csharp
public CellValueType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta valori di cella diversi con tipi diversi
            worksheet.Cells["A1"].PutValue("Text Value"); // Text type
            worksheet.Cells["A2"].PutValue(123.45);       // Numeric type
            worksheet.Cells["A3"].PutValue(true);        // Boolean type
            worksheet.Cells["A4"].PutValue("=1/0");       // Error type (will show #DIV/0!)

            // Elabora ogni cella e dimostra la proprietà Type
            for (int i = 0; i < 4; i++)
            {
                Cell cell = worksheet.Cells[0, i];
                CellValue value = (CellValue)cell.Value;
                
                Console.WriteLine($"Cell {cell.Name} - Original Type: {value.Type}, Value: {value.Value}");

                // Dimostra la modifica del tipo per i valori di errore
                if (value.Type == CellValueType.IsError && "#DIV/0!".Equals(value.Value))
                {
                    value.Type = CellValueType.IsNull;
                    Console.WriteLine($"Changed error to null - New Type: {value.Type}");
                }
            }
        }
    }
}
```

### Vedi anche

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


