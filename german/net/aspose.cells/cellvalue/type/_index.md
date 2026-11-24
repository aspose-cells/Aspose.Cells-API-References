---
title: "CellValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellValue-Eigenschaft. Gibt den Typ des Zellwerts zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Liest oder setzt den Typ des Zellenwerts.

```csharp
public CellValueType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze verschiedene Zellwerte mit unterschiedlichen Typen
            worksheet.Cells["A1"].PutValue("Text Value"); // Text type
            worksheet.Cells["A2"].PutValue(123.45);       // Numeric type
            worksheet.Cells["A3"].PutValue(true);        // Boolean type
            worksheet.Cells["A4"].PutValue("=1/0");       // Error type (will show #DIV/0!)

            // Verarbeite jede Zelle und demonstriere die Type‑Eigenschaft
            for (int i = 0; i < 4; i++)
            {
                Cell cell = worksheet.Cells[0, i];
                CellValue value = (CellValue)cell.Value;
                
                Console.WriteLine($"Cell {cell.Name} - Original Type: {value.Type}, Value: {value.Value}");

                // Demonstriere das Ändern des Typs für Fehlerwerte
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

### Siehe auch

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


