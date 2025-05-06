---
title: ChartCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Adds a chart to the collection
type: docs
url: /net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Adds a chart to the collection.

```csharp
public int Add(ChartType type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, 
    int lowerRightColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### Examples

```csharp
// Called: int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
public static void Method_Int32_()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(2);
            worksheet.Cells[&quot;A2&quot;].PutValue(5);
            worksheet.Cells[&quot;A3&quot;].PutValue(3);
            worksheet.Cells[&quot;A4&quot;].PutValue(6);
            worksheet.Cells[&quot;B1&quot;].PutValue(4);
            worksheet.Cells[&quot;B2&quot;].PutValue(3);
            worksheet.Cells[&quot;B3&quot;].PutValue(6);
            worksheet.Cells[&quot;B4&quot;].PutValue(7);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            worksheet.Cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Add a column chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Configure error bars for each series in the chart
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Save the workbook
            workbook.Save(&quot;ErrorBarDisplayTypeExample.xlsx&quot;);
            workbook.Save(&quot;ErrorBarDisplayTypeExample.pdf&quot;);
            return;
        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Adds a chart to the collection.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### Remarks

NOTE: This member is now obsolete. Instead, please use `Add` property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Adds a chart with preset template.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| data | Byte[] | The data of chart template file(.crtx). |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Adds a chart to the collection.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### Examples

```csharp
// Called: workbook.Worksheets[0].Charts.Add(ChartType.Column, &amp;quot;A1:D3&amp;quot;, true, 4, 4, 14, 10);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet50996.xlsx&quot;);
            workbook.Worksheets[0].Charts.Add(ChartType.Column, &quot;A1:D3&quot;, true, 4, 4, 14, 10);
            Assert.AreEqual(3, workbook.Worksheets[0].Charts[0].NSeries.Count);
            workbook.Save(Constants.destPath + &quot;CellsNet50996.xlsx&quot;);
        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


