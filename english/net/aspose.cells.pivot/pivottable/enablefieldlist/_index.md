---
title: PivotTable.EnableFieldList
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the field list for the PivotTable is available on the view of Excel
type: docs
url: /net/aspose.cells.pivot/pivottable/enablefieldlist/
---
## PivotTable.EnableFieldList property

Indicates whether the field list for the PivotTable is available on the view of Excel.

```csharp
public bool EnableFieldList { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.EnableFieldList, false);
public void PivotTable_Property_EnableFieldList()
{
    var wb = new Workbook(Constants.openPivottablePath + "dd.xls");
    PivotTable pt = wb.Worksheets[0].PivotTables[0];
    Assert.AreEqual(pt.EnableFieldList, false);
    //wb = new Workbook(Constants.openPivottablePath + "dd.xlsx");
    //pt = wb.Worksheets[0].PivotTables[0];

    //Assert.AreEqual(wb.Settings.HidePivotFieldList, true);
    wb = new Workbook(Constants.openPivottablePath + "AsposeIsIncludeNewItemsInFilter.xls");
    wb.Save(Constants.savePivottablePath + "example.xls");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


