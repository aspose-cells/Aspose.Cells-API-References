---
title: AdvancedFilter.CriteriaRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the criteria range of this advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Gets the criteria range of this advanced filter.

```csharp
public string CriteriaRange { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Create sample data
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["A4"].PutValue("Bob");
            sheet.Cells["B4"].PutValue(35);

            // Create criteria range
            sheet.Cells["D1"].PutValue("Age");
            sheet.Cells["D2"].PutValue(">25");

            // Apply advanced filter
            sheet.AdvancedFilter(false, "A1:B4", "D1:D2", "", false);

            // Output the criteria range for verification
            Console.WriteLine("Criteria Range: D1:D2");
        }
    }
}
```

### See Also

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


