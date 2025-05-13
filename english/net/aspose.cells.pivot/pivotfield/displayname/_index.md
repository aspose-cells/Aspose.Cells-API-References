---
title: PivotField.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the PivotField display name
type: docs
url: /net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Represents the PivotField display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: Cell cell = pivotTable.GetCellByDisplayName(pivotTable.DataFields[2].DisplayName);
public void PivotField_Property_DisplayName()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43367_";
    var workbook = new Workbook(filePath + "example2.xlsx");
    var worksheet = workbook.Worksheets[0];
    var pivotTable = worksheet.PivotTables[0];

    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = false;

    Style style = workbook.CreateStyle();
    style.BackgroundColor = Color.Yellow;
    style.Pattern = BackgroundType.Solid;
    Cell cell = pivotTable.GetCellByDisplayName(pivotTable.DataFields[2].DisplayName);

    int preColor = cell.GetStyle().ForegroundArgbColor;
    pivotTable.Format(cell.Row, cell.Column, style);
    Assert.AreNotEqual(preColor, cell.GetStyle().ForegroundArgbColor);
    workbook.Save(Constants.PivotTableDestPath + @"example.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


