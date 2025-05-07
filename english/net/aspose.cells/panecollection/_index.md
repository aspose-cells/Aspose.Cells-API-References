---
title: Class PaneCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.PaneCollection class. Represents all Pane objects shown in the specified window
type: docs
url: /net/aspose.cells/panecollection/
---
## PaneCollection class

Represents all Pane objects shown in the specified window.

```csharp
public class PaneCollection
```

## Properties

| Name | Description |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | Gets and sets the active pane. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Gets and sets the first visible column of the right pane. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Gets and sets the first visible row of the bottom pane. |

### Examples

```csharp
// Called: PaneCollection panes = sheet.GetPanes();
[Test]
        public void Type_PaneCollection()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


