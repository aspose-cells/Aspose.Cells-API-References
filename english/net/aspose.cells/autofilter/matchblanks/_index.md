---
title: AutoFilter.MatchBlanks
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Match all blank cells in the list
type: docs
url: /net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Match all blank cells in the list.

```csharp
public void MatchBlanks(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data with some blank cells
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Leave C2 blank
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Leave B3 blank
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Apply auto filter
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filter to show only rows with blanks in column 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Refresh the filter
            filter.Refresh();
            
            // Save the workbook
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


