---
title: "PivotTable.IsGridDropZones"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable-rapporten visar klassisk pivottabelllayout. möjliggör dragning av fält i rutnätet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Anger om PivotTable‑rapporten visar klassisk pivottable‑layout. (möjliggör att dra fält i rutnätet)

```csharp
public bool IsGridDropZones { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsGridDropZonesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Ställ in egenskapen IsGridDropZones
            pivotTable.IsGridDropZones = true;
            Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);

            // Spara arbetsboken
            workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


