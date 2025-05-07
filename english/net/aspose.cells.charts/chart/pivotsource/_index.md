---
title: Chart.PivotSource
second_title: Aspose.Cells for .NET API Reference
description: Chart property. The source is the data of the pivotTable. If PivotSource is not empty the chart is PivotChart
type: docs
url: /net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Remarks

If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### Examples

```csharp
// Called: Assert.AreEqual("New' Name!PivotTable1", wb.Worksheets[0].Charts[0].PivotSource, "Chart.PivotSource");
[Test]
        public void Property_PivotSource()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Charts/N46097.xlsx");
            Cell cell = wb.Worksheets[0].Cells[4, 3];
            cell.Value = 3;
            // Rename the sheet using a name with ' 
            wb.Worksheets[0].Name = "New' Name";
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            Assert.AreEqual("New' Name!PivotTable1", wb.Worksheets[0].Charts[0].PivotSource, "Chart.PivotSource");
            wb.Worksheets[0].Charts[0].RefreshPivotData();//Exception 
            Util.ReSave(wb, SaveFormat.Xlsx);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


