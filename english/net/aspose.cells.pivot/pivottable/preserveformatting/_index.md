---
title: PivotTable.PreserveFormatting
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether cell formatting PivotTableFormat is preserved when the PivotTable is refreshed or recalculated
type: docs
url: /net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Indicates whether cell formatting ([`PivotTableFormat`](../../pivottableformat/)) is preserved when the PivotTable is refreshed or recalculated.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotTable.PreserveCellFormattingOnUpdate property. This method will be removed 12 months later since July 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("source.xlsx");
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the first pivot table
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Enable preserving formatting during refresh
            pivotTable.PreserveFormatting = true;
            
            // Apply some formatting to pivot table data area
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Format the pivot table data area
            pivotTable.FormatAll(style);
            
            // Refresh and calculate pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Save the workbook
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


