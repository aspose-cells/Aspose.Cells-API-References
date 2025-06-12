---
title: Class AdvancedFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AdvancedFilter class. Represents the settings of advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Represents the settings of advanced filter.

```csharp
public class AdvancedFilter
```

## Properties

| Name | Description |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Gets the range where copying the resut of this advanced filter to. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Gets the criteria range of this advanced filter. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Gets the list range of this advanced filter. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterDemo
    {
        public static void AdvancedFilterExample()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate data for the list range
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);
            worksheet.Cells["A5"].PutValue("Emily");
            worksheet.Cells["B5"].PutValue(35);

            // Populate criteria range
            worksheet.Cells["D1"].PutValue("Age");
            worksheet.Cells["D2"].PutValue(">25");

            // Applying advanced filter
            //CellArea listRange = CellArea.CreateCellArea("A1", "B5");
            //CellArea criteriaRange = CellArea.CreateCellArea("D1", "D2");
            //CellArea copyToRange = CellArea.CreateCellArea("F1", "G1");

            worksheet.AdvancedFilter(true, "A1:B5", "D1:D2", "", false);

            // Save the workbook
            workbook.Save("AdvancedFilterExample2.xlsx");
            workbook.Save("AdvancedFilterExample2.pdf");

            //worksheet.AdvancedFilter(false, "A1:B5", "D1:D2", "F1:G5", false);

            //// Save the workbook
            //workbook.Save("AdvancedFilterExample.xlsx");
            //workbook.Save("AdvancedFilterExample.pdf");


            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


