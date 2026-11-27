---
title: "PivotFilter.FieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar indexet för källfältet som detta pivottfilter tillämpas på"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Hämtar indexet för källfältet som detta pivotfilter tillämpas på.

```csharp
public int FieldIndex { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFieldIndexDemo
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
            cells["B4"].Value = 8;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till filter
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField pivotField = pivotTable.PageFields[0];
            
            // Skapa pivottfiltersamling och lägg till filter
            PivotFilterCollection filters = pivotTable.PivotFilters;
            int filterIndex = filters.Add(0, PivotFilterType.Count);
            PivotFilter filter = filters[filterIndex];
            
            // Demonstrera FieldIndex-egenskapen
            Console.WriteLine("Field Index: " + filter.FieldIndex);

            // Spara arbetsboken
            workbook.Save("PivotFilterFieldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


