---
title: "FindOptions.SetRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-metod. Anger det sökta intervallet"
type: docs
url: /sv/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Anger det sökta intervallet.

```csharp
public void SetRange(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | det sökta intervallet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // Skapa FindOptions och ange sökintervallet
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Sök inom det angivna intervallet
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


