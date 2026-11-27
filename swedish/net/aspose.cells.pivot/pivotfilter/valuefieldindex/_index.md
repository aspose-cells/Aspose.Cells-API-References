---
title: "PivotFilter.ValueFieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar indexet för värdefältet i värdeområdet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

Hämtar indexet för värdefältet i värdeområdet.

```csharp
public int ValueFieldIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValueFieldIndexDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
            
            // Lägg till räknefilter till radfältet
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Hämta filtret och demonstrera ValueFieldIndex
            PivotFilter filter = rowField.GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            
            // Spara arbetsboken
            workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


