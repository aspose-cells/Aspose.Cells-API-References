---
title: Class MultipleFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MultipleFilterCollection class. Represents the multiple filter collection
type: docs
url: /net/aspose.cells/multiplefiltercollection/
---
## MultipleFilterCollection class

Represents the multiple filter collection.

```csharp
public class MultipleFilterCollection : CollectionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [MultipleFilterCollection](multiplefiltercollection/)() | Constructs one new instance. |

## Properties

| Name | Description |
| --- | --- |
| [Item](../../aspose.cells/multiplefiltercollection/item/) { get; } | Gets [`DateTimeGroupItem`](../datetimegroupitem/) or a string value. |
| [MatchBlank](../../aspose.cells/multiplefiltercollection/matchblank/) { get; set; } | Indicates whether to filter by blank. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/multiplefiltercollection/add/#add_1)(string) | Adds a label filter. |
| [Add](../../aspose.cells/multiplefiltercollection/add/#add)(DateTimeGroupingType, int, int, int) | Adds a date filter criteria value. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMultipleFilterCollectionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate sample data
            cells[0, 0].PutValue("Data");
            cells[1, 0].PutValue("abc");
            cells[2, 0].PutValue("def");
            cells[3, 0].PutValue("ghi");
            cells[4, 0].PutValue("abc");
            cells[5, 0].PutValue("jkl");
            cells[6, 0].PutValue("mno");

            // Apply auto filter
            sheet.AutoFilter.Range = "A1:A7";
            FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
            fc.FilterType = FilterType.MultipleFilters;

            // Create and configure multiple filter collection
            MultipleFilterCollection mfc = new MultipleFilterCollection();
            mfc.Add("abc");
            mfc.Add("ghi");
            mfc.MatchBlank = false;
            fc.Filter = mfc;

            // Apply filter
            sheet.AutoFilter.Refresh();

            // Display results
            Console.WriteLine("Filter Results:");
            for (int i = 1; i <= 6; i++)
            {
                Console.WriteLine($"Row {i}: {(cells.IsRowHidden(i) ? "Hidden" : "Visible")}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


