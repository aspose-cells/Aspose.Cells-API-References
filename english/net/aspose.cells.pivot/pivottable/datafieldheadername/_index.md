---
title: PivotTable.DataFieldHeaderName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the name of the value area field header in the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/datafieldheadername/
---
## PivotTable.DataFieldHeaderName property

Gets and sets the name of the value area field header in the PivotTable.

```csharp
public string DataFieldHeaderName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("AsposeValues", pivot.DataFieldHeaderName);
public void PivotTable_Property_DataFieldHeaderName()
{
    Workbook book = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    book.Settings.GlobalizationSettings.PivotSettings = new CustomPivotTableGlobalizationSettings_53714();

    PivotTable pivot = book.Worksheets[0].PivotTables[0];
           
    // pivot.DataField.DisplayName = "asfdsfsf";
    pivot.DataFields[0].DisplayName = "Abc";
    pivot.RefreshData();
    pivot.CalculateData();
           
    Assert.AreEqual("a1 Abc", book.Worksheets[0].Cells["B12"].StringValue);
    Assert.AreEqual("AsposeValues", pivot.DataFieldHeaderName);
    book.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


