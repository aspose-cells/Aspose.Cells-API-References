---
title: Chart.RefreshPivotData
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Refreshes charts data from pivot table
type: docs
url: /net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Refreshes chart's data from pivot table.

```csharp
public void RefreshPivotData()
```

### Remarks

We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.

### Examples

```csharp
// Called: charts[j].RefreshPivotData();
[Test]
        public void Method_RefreshPivotData()
        {
            String filePath = Constants.PivotTableSourcePath + @"JAVA41968_";

            Workbook workbook = new Workbook(filePath + "aspose.xlsx");
            ChartCollection charts = workbook.Worksheets["Tabelle2"].Charts;
            for (int j = 0; j < charts.Count; j++)
            {
                charts[j].RefreshPivotData();
                charts[j].Calculate();
            }

            workbook.Save(Constants.PivotTableDestPath + @"JAVA41968_" + "out.pdf");
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


