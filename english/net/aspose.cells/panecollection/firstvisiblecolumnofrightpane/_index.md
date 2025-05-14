---
title: PaneCollection.FirstVisibleColumnOfRightPane
second_title: Aspose.Cells for .NET API Reference
description: PaneCollection property. Gets and sets the first visible column of the right pane
type: docs
url: /net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Gets and sets the first visible column of the right pane.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Examples

```csharp
// Called: panes.FirstVisibleColumnOfRightPane = 1;
public void PaneCollection_Property_FirstVisibleColumnOfRightPane()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet sheet = workbook.Worksheets["MonSumSheet1"];
    PaneCollection panes = sheet.GetPanes();
    panes.FirstVisibleRowOfBottomPane = 5;
    panes.FirstVisibleColumnOfRightPane = 1;
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


