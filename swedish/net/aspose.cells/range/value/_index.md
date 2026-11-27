---
title: "Range.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar och anger värdet för området"
type: docs
url: /sv/net/aspose.cells/range/value/
---
## Range.Value property

Hämtar och anger värdet för området.

```csharp
public object Value { get; set; }
```

### Anmärkningar

Om området innehåller flera celler ska det returnerade/verkställda objektet vara ett tvådimensionellt Array-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett område som startar från A1 och täcker 3x3 celler
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Ange en 2D-array som värde för området
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Spara arbetsboken
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


