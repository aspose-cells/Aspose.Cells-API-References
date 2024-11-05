---
title: Enum PivotFilterType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFilterType enum. Represents PivotTable Filter type
type: docs
url: /net/aspose.cells.pivot/pivotfiltertype/
---
## PivotFilterType enumeration

Represents PivotTable Filter type.

```csharp
public enum PivotFilterType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| CaptionBeginsWith | `0` | Indicates the "begins with" filter for field captions. |
| CaptionBetween | `1` | Indicates the "is between" filter for field captions. |
| CaptionContains | `2` | Indicates the "contains" filter for field captions. |
| CaptionEndsWith | `3` | Indicates the "ends with" filter for field captions. |
| CaptionEqual | `4` | Indicates the "equal" filter for field captions. |
| CaptionGreaterThan | `5` | Indicates the "is greater than" filter for field captions. |
| CaptionGreaterThanOrEqual | `6` | Indicates the "is greater than or equal to" filter for field captions. |
| CaptionLessThan | `7` | Indicates the "is less than" filter for field captions. |
| CaptionLessThanOrEqual | `8` | Indicates the "is less than or equal to" filter for field captions. |
| CaptionNotBeginsWith | `9` | Indicates the "does not begin with" filter for field captions. |
| CaptionNotBetween | `10` | Indicates the "is not between" filter for field captions. |
| CaptionNotContains | `11` | Indicates the "does not contain" filter for field captions. |
| CaptionNotEndsWith | `12` | Indicates the "does not end with" filter for field captions. |
| CaptionNotEqual | `13` | Indicates the "not equal" filter for field captions. |
| Count | `14` | Indicates the "count" filter. |
| DateBetween | `15` | Indicates the "between" filter for date values. |
| DateEqual | `16` | Indicates the "equals" filter for date values. |
| DateNewerThan | `17` | Indicates the "newer than" filter for date values. |
| DateNewerThanOrEqual | `18` | Indicates the "newer than or equal to" filter for date values. |
| DateNotBetween | `19` | Indicates the "not between" filter for date values. |
| DateNotEqual | `20` | Indicates the "does not equal" filter for date values. |
| DateOlderThan | `21` | Indicates the "older than" filter for date values. |
| DateOlderThanOrEqual | `22` | Indicates the "older than or equal to" filter for date values. |
| LastMonth | `23` | Indicates the "last month" filter for date values. |
| LastQuarter | `24` | Indicates the "last quarter" filter for date values. |
| LastWeek | `25` | Indicates the "last week" filter for date values. |
| LastYear | `26` | Indicates the "last year" filter for date values. |
| M1 | `27` | Indicates the "January" filter for date values. |
| M2 | `28` | Indicates the "February" filter for date values. |
| M3 | `29` | Indicates the "March" filter for date values. |
| M4 | `30` | Indicates the "April" filter for date values. |
| M5 | `31` | Indicates the "May" filter for date values. |
| M6 | `32` | Indicates the "June" filter for date values. |
| M7 | `33` | Indicates the "July" filter for date values. |
| M8 | `34` | Indicates the "August" filter for date values. |
| M9 | `35` | Indicates the "September" filter for date values. |
| M10 | `36` | Indicates the "October" filter for date values. |
| M11 | `37` | Indicates the "November" filter for date values. |
| M12 | `38` | Indicates the "December" filter for date values. |
| NextMonth | `39` | Indicates the "next month" filter for date values. |
| NextQuarter | `40` | Indicates the "next quarter" for date values. |
| NextWeek | `41` | Indicates the "next week" for date values. |
| NextYear | `42` | Indicates the "next year" filter for date values. |
| Percent | `43` | Indicates the "percent" filter for numeric values. |
| Q1 | `44` | Indicates the "first quarter" filter for date values. |
| Q2 | `45` | Indicates the "second quarter" filter for date values. |
| Q3 | `46` | Indicates the "third quarter" filter for date values. |
| Q4 | `47` | Indicates the "fourth quarter" filter for date values. |
| Sum | `48` | Indicates the "sum" filter for numeric values. |
| ThisMonth | `49` | Indicates the "this month" filter for date values. |
| ThisQuarter | `50` | Indicates the "this quarter" filter for date values. |
| ThisWeek | `51` | Indicates the "this week" filter for date values. |
| ThisYear | `52` | Indicate the "this year" filter for date values. |
| Today | `53` | Indicates the "today" filter for date values. |
| Tomorrow | `54` | Indicates the "tomorrow" filter for date values. |
| Unknown | `55` | Indicates the PivotTable filter is unknown to the application. |
| ValueBetween | `56` | Indicates the "Value between" filter for text and numeric values. |
| ValueEqual | `57` | Indicates the "value equal" filter for text and numeric values. |
| ValueGreaterThan | `58` | Indicates the "value greater than" filter for text and numeric values. |
| ValueGreaterThanOrEqual | `59` | Indicates the "value greater than or equal to" filter for text and numeric values. |
| ValueLessThan | `60` | Indicates the "value less than" filter for text and numeric values. |
| ValueLessThanOrEqual | `61` | Indicates the "value less than or equal to" filter for text and numeric values. |
| ValueNotBetween | `62` | Indicates the "value not between" filter for text and numeric values. |
| ValueNotEqual | `63` | Indicates the "value not equal" filter for text and numeric values. |
| YearToDate | `64` | Indicates the "year-to-date" filter for date values. |
| Yesterday | `65` | Indicates the "yesterday" filter for date values. |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterTypeDemo
    {
        public static void PivotFilterTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add some data to the worksheet
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Add a PivotTable to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Set PivotTable style
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add a PivotFilter to the PivotTable
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionContains);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Refresh and calculate the PivotTable data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotFilterTypeExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


