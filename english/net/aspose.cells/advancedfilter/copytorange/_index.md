---
title: AdvancedFilter.CopyToRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the range where copying the resut of this advanced filter to
type: docs
url: /net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Gets the range where copying the resut of this advanced filter to.

```csharp
public string CopyToRange { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data for filtering
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("Sales");
            sheet.Cells["A3"].PutValue("HR");
            sheet.Cells["A4"].PutValue("IT");
            sheet.Cells["A5"].PutValue("Sales");
            
            // Create criteria range
            sheet.Cells["C1"].PutValue("Department");
            sheet.Cells["C2"].PutValue("Sales");
            
            // Initialize advanced filter with all required parameters
            sheet.AdvancedFilter(false, "A1:A5", "C1:C2", "E1", true);
            
            // Save the workbook
            workbook.Save("AdvancedFilterCopyToRangeDemo.xlsx");
        }
    }
}
```

### See Also

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


