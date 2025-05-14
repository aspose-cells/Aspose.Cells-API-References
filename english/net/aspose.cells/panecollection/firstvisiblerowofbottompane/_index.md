---
title: PaneCollection.FirstVisibleRowOfBottomPane
second_title: Aspose.Cells for .NET API Reference
description: PaneCollection property. Gets and sets the first visible row of the bottom pane
type: docs
url: /net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Gets and sets the first visible row of the bottom pane.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2,workbook.Worksheets[0].GetPanes().FirstVisibleRowOfBottomPane);
public void PaneCollection_Property_FirstVisibleRowOfBottomPane()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].Cells.DeleteRow(0);
    Assert.AreEqual(2,workbook.Worksheets[0].GetPanes().FirstVisibleRowOfBottomPane);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


