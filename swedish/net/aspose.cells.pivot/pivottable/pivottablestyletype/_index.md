---
title: "PivotTable.PivotTableStyleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger den inbyggda pivottabellstilen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Hämtar och anger den inbyggda pivottabellstilen.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ställ in och demonstrera PivotTableStyleType
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);

            // Spara arbetsboken
            workbook.Save("PivotTableStyleTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


