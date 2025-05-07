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
// Called: panes.FirstVisibleRowOfBottomPane = 5;
[Test]
        public void Property_FirstVisibleRowOfBottomPane()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet14240.xls");
            Worksheet sheet = workbook.Worksheets["MonSumSheet1"];
            PaneCollection panes = sheet.GetPanes();
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + "CellsNet14240.xls");
        }
```

### See Also

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


