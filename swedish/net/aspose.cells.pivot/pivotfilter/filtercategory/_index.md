---
title: "PivotFilter.FilterCategory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter egenskap. Hämtar kategorin för detta filter"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/filtercategory/
---
## PivotFilter.FilterCategory property

Hämtar kategorin för detta filter.

```csharp
public FilterCategory FilterCategory { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyFilterCategoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa exempeldata för pivottabell
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                worksheet.Cells["B1"].Value = "Value";
                worksheet.Cells["B2"].Value = 100;
                worksheet.Cells["B3"].Value = 200;
                worksheet.Cells["B4"].Value = 300;

                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Lägg till radfält med korrekt API-metod
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                
                // Lägg till datafält med korrekt API-metod
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;
                dataField.DisplayName = "Total";

                // Lägg till rubrikfilter till Kategori-fältet
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Visa värdet för FilterCategory-egenskapen
                Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);

                workbook.Save("FilterCategoryDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


