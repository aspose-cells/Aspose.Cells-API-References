---
title: PivotField.AutoSortField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the index of field which is auto sorted. 1 means PivotField itselfothers means the position of the data fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

```csharp
public int AutoSortField { get; set; }
```

### Examples

```csharp
// Called: pivotField.AutoSortField = 0;
public void PivotField_Property_AutoSortField()
{
    string filePath = Constants.PivotTableSourcePath + @"NET42556_";

    var book = new Aspose.Cells.Workbook(filePath + "example.xls");
    var sheet = book.Worksheets[0];
    var pivot = sheet.PivotTables[0];

    PivotFieldCollection pivotFields = pivot.BaseFields;

    PivotField pivotField = pivotFields["Branch"];

    //Setting the field auto sort
    pivotField.IsAutoSort = true;

    //Setting the field sorting in ascending order
    pivotField.IsAscendSort = true;

    //Sort PivotField named "Branch" via DataField named "GPW"
    pivotField.AutoSortField = 0;

    pivot.CalculateData();
    pivot.RefreshDataOnOpeningFile = true;

    string savePath = CreateFolder(filePath);
    book.Save(savePath + "out.xlsx");
    book.Save(savePath + "out.pdf");

}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


