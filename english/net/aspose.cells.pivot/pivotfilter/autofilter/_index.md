---
title: PivotFilter.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Gets the autofilter of the pivot filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

Gets the autofilter of the pivot filter.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### Remarks

NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add sample data
            cells["A1"].Value = "Data";
            cells["A2"].Value = 10;
            cells["A3"].Value = 20;
            cells["A4"].Value = 30;
            cells["A5"].Value = 40;
            cells["A6"].Value = 50;

            // Apply AutoFilter to the range
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Demonstrate AutoFilter property by filtering top 2 items
            filter.FilterTop10(0, false, false, 2);

            // Save the workbook
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


