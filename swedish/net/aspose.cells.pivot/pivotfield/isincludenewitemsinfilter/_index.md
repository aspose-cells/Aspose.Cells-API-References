---
title: "PivotField.IsIncludeNewItemsInFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om nya objekt ska inkluderas i fältet i ett manuellt filter. Standardvärdet är false."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Anger om nya objekt ska inkluderas i fältet i manuellt filter. Standardvärdet är false.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsIncludeNewItemsInFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivotfältet och ställ in IsIncludeNewItemsInFilter
            PivotField field = pivotTable.RowFields[0];
            field.IsIncludeNewItemsInFilter = true;
            
            // Skriv ut egenskapsvärdet
            Console.WriteLine("IsIncludeNewItemsInFilter: " + field.IsIncludeNewItemsInFilter);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldPropertyIsIncludeNewItemsInFilterDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


