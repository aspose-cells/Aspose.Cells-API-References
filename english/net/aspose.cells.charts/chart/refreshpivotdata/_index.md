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
// Called: chart.RefreshPivotData();
public void Chart_Method_RefreshPivotData()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA41851_";

    //Instantiating an Workbook object 
    Workbook workbook = new Workbook(filePath + "foo.xlsx");
    //Adding a column chart 
    int chartIndex = workbook.Worksheets["Pivot"].Charts.Add(ChartType.Column, 10, 6, 28, 16);
    Chart chart = workbook.Worksheets["Pivot"].Charts[chartIndex];
    //Setting the pivot chart data source 
    chart.PivotSource = "Pivot!IF_Pivot";
    chart.HidePivotFieldButtons = true;
    chart.RefreshPivotData();
    //Saving the Excel file 
    chart.PivotSource = null;
    workbook.Save(Constants.PivotTableDestPath + @"example.xlsx");
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


