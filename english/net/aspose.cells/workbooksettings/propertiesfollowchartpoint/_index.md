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
// Called: workbook.Settings.PropertiesFollowChartPoint = true;
[Test]
        public void Property_PropertiesFollowChartPoint()
        {

            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet57038.xlsx&quot;);
            //CELLSNET-57042
            workbook.Settings.PropertiesFollowChartPoint = true;
            // Save the workbook
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsx&quot;);
            bool c = ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + @&quot;CellsNet57038.xlsx&quot;, &quot;xl/pivotTables/pivotTable1.xml&quot;, new string[] { &quot;e=\&quot;0\&quot;&quot; }, true);
            Assert.IsTrue(c);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsx&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsb&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsb&quot;);
            Assert.IsTrue(workbook.Settings.PropertiesFollowChartPoint);

        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


