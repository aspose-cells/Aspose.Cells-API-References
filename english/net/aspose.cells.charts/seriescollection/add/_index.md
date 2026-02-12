---
title: SeriesCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Adds the Series collection to a chart
type: docs
url: /net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Adds the [`Series`](../../series/) collection to a chart.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataArea | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. If true, [`Series`](../../series/) will be added column by column |

### Return Value

Return the first index of the added ASeries in the NSeries.

### Remarks

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).This method only simply process *dataArea* as data range. If you want to smartly check ChartCollection.Add() method.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Create chart
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Add series using string and boolean parameters
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Save the workbook
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Adds the [`Series`](../../series/) collection to a chart.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | Boolean | Indicates whether the range contains series's name |

### Return Value

Return the first index of the added ASeries in the NSeries.

### Remarks

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Create chart
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Add series using the Add method with string and boolean parameters
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Save the workbook
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


