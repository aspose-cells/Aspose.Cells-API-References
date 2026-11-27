---
title: "CellValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellValue‑egenskap. Hämtar eller anger typen av cellvärde"
type: docs
url: /sv/net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Hämtar eller anger typen av cellvärde.

```csharp
public CellValueType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange olika cellvärden med olika typer
            worksheet.Cells["A1"].PutValue("Text Value"); // Text type
            worksheet.Cells["A2"].PutValue(123.45);       // Numeric type
            worksheet.Cells["A3"].PutValue(true);        // Boolean type
            worksheet.Cells["A4"].PutValue("=1/0");       // Error type (will show #DIV/0!)

            // Bearbeta varje cell och demonstrera Type‑egenskapen
            for (int i = 0; i < 4; i++)
            {
                Cell cell = worksheet.Cells[0, i];
                CellValue value = (CellValue)cell.Value;
                
                Console.WriteLine($"Cell {cell.Name} - Original Type: {value.Type}, Value: {value.Value}");

                // Demonstrera ändring av typ för felvärden
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

### Se även

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


