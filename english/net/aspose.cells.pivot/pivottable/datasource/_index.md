---
title: PivotTable.DataSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the data source of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Gets and sets the data source of the pivot table.

```csharp
public string[] DataSource { get; set; }
```

### Examples

```csharp
// Called: var dataSource = pivotTable.DataSource; // throws exception
public void PivotTable_Property_DataSource()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    var pivotTable = wb.Worksheets[0].PivotTables[0];
    var dataSource = pivotTable.DataSource; // throws exception
    Assert.AreEqual("tbl_Scenario_Data_Annual",dataSource[1]);
    Assert.AreEqual("tbl_Years", dataSource[0]);
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


