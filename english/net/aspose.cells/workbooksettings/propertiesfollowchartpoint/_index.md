---
title: WorkbookSettings.PropertiesFollowChartPoint
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference
type: docs
url: /net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.PropertiesFollowChartPoint);
public void WorkbookSettings_Property_PropertiesFollowChartPoint()
{

    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    //CELLSNET-57042
    workbook.Settings.PropertiesFollowChartPoint = true;
    // Save the workbook
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    bool c = ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + @"example.xlsx", "xl/pivotTables/pivotTable1.xml", new string[] { "e=\"0\"" }, true);
    Assert.IsTrue(c);
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    workbook.Save(Constants.PivotTableDestPath + "example.xlsb");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsb");
    Assert.IsTrue(workbook.Settings.PropertiesFollowChartPoint);

}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


