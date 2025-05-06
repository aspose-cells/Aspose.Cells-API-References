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
[Test]
        public void Property_FirstVisibleColumnOfRightPane()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet14240.xls&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;MonSumSheet1&quot;];
            PaneCollection panes = sheet.GetPanes();
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + &quot;CellsNet14240.xls&quot;);
        }
```

### See Also

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


