---
title: PivotField.ShowValuesSetting
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the settings of showing values as when the ShowDataAs calculation is in use
type: docs
url: /net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Gets the settings of showing values as when the ShowDataAs calculation is in use.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Examples

```csharp
// Called: field.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
public void PivotField_Property_ShowValuesSetting()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.DataFields[0];
    field.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("4.39%", cells["C33"].StringValue);
    book.Save(Constants.destPath + "TestShowValuesSetting.xlsx");

}
```

### See Also

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


