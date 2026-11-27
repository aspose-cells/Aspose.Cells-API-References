---
title: "PivotFilter.MemberPropertyFieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar medlemsegenskapsfältets index för pivottfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/
---
## PivotFilter.MemberPropertyFieldIndex property

Hämtar medlemsegenskapsfältets index för pivotfiltret.

```csharp
public int MemberPropertyFieldIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMemberPropertyFieldIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ställ in exempeldata
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["A2"].Value = "Fruit";
            sheet.Cells["A3"].Value = "Vegetable";
            sheet.Cells["A4"].Value = "Fruit";
            sheet.Cells["A5"].Value = "Vegetable";
            
            sheet.Cells["B1"].Value = "Product";
            sheet.Cells["B2"].Value = "Apple";
            sheet.Cells["B3"].Value = "Carrot";
            sheet.Cells["B4"].Value = "Banana";
            sheet.Cells["B5"].Value = "Potato";
            
            sheet.Cells["C1"].Value = "Price";
            sheet.Cells["C2"].Value = 10;
            sheet.Cells["C3"].Value = 5;
            sheet.Cells["C4"].Value = 8;
            sheet.Cells["C5"].Value = 3;

            // Skapa pivottabell – åtgärdad genom att hämta pivottabellen från samlingen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            
            // Lägg till pivottfilter och sätt MemberPropertyFieldIndex
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MemberPropertyFieldIndex = 1; // Using Product field as member property
            
            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotFilterWithMemberPropertyFieldIndex.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


