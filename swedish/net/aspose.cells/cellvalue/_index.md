---
title: "Klass CellValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellValue-klass. Representerar cellvärdet och motsvarande typ"
type: docs
url: /sv/net/aspose.cells/cellvalue/
---
## CellValue class

Representerar cellvärdet och motsvarande typ.

```csharp
public class CellValue
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CellValue](cellvalue/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Hämtar eller anger typen av cellvärde. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Hämtar eller anger cellvärdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en CellValue-instans
            CellValue cellValue = new CellValue();

            // Ange typen och värdet för cellen
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Tilldela CellValue till en cell i kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Spara arbetsboken
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


