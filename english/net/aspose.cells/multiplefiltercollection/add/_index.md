---
title: MultipleFilterCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: MultipleFilterCollection method. Adds a label filter criteria
type: docs
url: /net/aspose.cells/multiplefiltercollection/add/
---
## Add(string) {#add_2}

Adds a label filter criteria.

```csharp
public void Add(string filter)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filter | String | The filter data. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MultipleFilterCollectionMethodAddWithStringDemo
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
            
            // Apply filter
            sheet.AutoFilter.Range = "A1:A5";
            FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
            fc.FilterType = FilterType.MultipleFilters;
            
            MultipleFilterCollection mfc = new MultipleFilterCollection();
            mfc.Add("abc");  // Demonstrate Add method with string parameter
            mfc.Add("ghi");
            
            fc.Filter = mfc;
            sheet.AutoFilter.Refresh();
            
            // Output filtered results
            Console.WriteLine("Filtered Rows:");
            for (int i = 1; i <= 4; i++)
            {
                if (!cells.IsRowHidden(i))
                {
                    Console.WriteLine(cells[i, 0].StringValue);
                }
            }
        }
    }
}
```

### See Also

* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DateTimeGroupingType, int, int, int) {#add}

Adds a date filter criteria value.

```csharp
public void Add(DateTimeGroupingType type, int year, int month, int day)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | DateTimeGroupingType | The type of date filter. |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DateTimeGroupingType, int, int, int, int, int, int) {#add_1}

Adds a date time filter criteria value.

```csharp
public void Add(DateTimeGroupingType type, int year, int month, int day, int hour, int minute, 
    int second)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | DateTimeGroupingType | The type of date filter. |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |
| hour | Int32 | The hour. |
| minute | Int32 | The minute. |
| second | Int32 | The second. |

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


