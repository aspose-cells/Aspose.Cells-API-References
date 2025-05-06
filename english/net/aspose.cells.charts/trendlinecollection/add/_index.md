---
title: TrendlineCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: TrendlineCollection method. Adds a Trendline object to this collection with specified type
type: docs
url: /net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Adds a [`Trendline`](../../trendline/) object to this collection with specified type.

```csharp
public int Add(TrendlineType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |

### Return Value

[`Trendline`](../../trendline/) object index.

### Examples

```csharp
// Called: chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
[Test]
        public void Method_TrendlineType_()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            checkTrendlineType_Exponential(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTrendlineType_Exponential(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTrendlineType_Exponential(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Adds a [`Trendline`](../../trendline/) object to this collection with specified type and name.

```csharp
public int Add(TrendlineType type, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |
| name | String | Trendline name. |

### Return Value

[`Trendline`](../../trendline/) object index.

### Examples

```csharp
// Called: int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, &amp;quot;MyTrendLine&amp;quot;);
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(200);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            worksheet.Cells[&quot;B4&quot;].PutValue(40);

            // Adding a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B4&quot;
            chart.NSeries.Add(&quot;A1:A4&quot;, true);
            chart.NSeries.Add(&quot;B1:B4&quot;, true);
            
            // Adding a trendline to the first series
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, &quot;MyTrendLine&quot;);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Setting trendline properties
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Saving the Excel file
            workbook.Save(&quot;TrendlineCollectionExample.xlsx&quot;);
        }
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


