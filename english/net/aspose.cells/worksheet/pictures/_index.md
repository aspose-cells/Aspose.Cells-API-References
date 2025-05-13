---
title: Worksheet.Pictures
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a Picture collection
type: docs
url: /net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Gets a [`Picture`](../../../aspose.cells.drawing/picture/) collection.

```csharp
public PictureCollection Pictures { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].Pictures.Count);
public void Worksheet_Property_Pictures()
{
    string file = Constants.sourcePath + "example.xls";
    LoadOptions loadOptions = new LoadOptions(LoadFormat.Excel97To2003);
    Workbook workbook = new Workbook(file, loadOptions);
    Assert.AreEqual(1, workbook.Worksheets[0].Pictures.Count);
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual(1, cells[0, 0].IntValue);
    Assert.AreEqual(true, cells[2, 0].BoolValue);
    Assert.AreEqual("=SUM(A1:A2)", cells[4, 0].Formula);
    Assert.AreEqual(true, cells[6, 0].IsStyleSet);
    Assert.AreEqual("Test", cells[0, 2].StringValue);
}
```

### See Also

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


