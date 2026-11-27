---
title: "Cell.GetStringValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar strängvärdet med en specifik formateringsstrategi"
type: docs
url: /sv/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Hämtar strängvärdet med en specifik formateringsstrategi.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | Den formaterade strategin. |

### Exempel

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

            // Ange olika typer av data i celler
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // Demonstrera GetStringValue med olika formateringsstrategier
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### Se även

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


