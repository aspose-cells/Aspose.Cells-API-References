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
// Called: chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
[Test]
        public void Method_TrendlineType_()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);  

            checkTrendlineType_Linear(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTrendlineType_Linear(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTrendlineType_Linear(workbook);
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
// Called: int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Adding a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // Adding a trendline to the first series
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Setting trendline properties
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Saving the Excel file
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


