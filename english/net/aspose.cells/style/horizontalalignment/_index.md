---
title: Style.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the horizontal alignment type of the text in a cell
type: docs
url: /net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Gets or sets the horizontal alignment type of the text in a cell.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: style.HorizontalAlignment = TextAlignmentType.CenterAcross;
[Test]
        public void Property_HorizontalAlignment()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[1, 1].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.CenterAcross;
            cells[1, 1].SetStyle(style);

            checkTextAlignmentType_CenterAcross(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTextAlignmentType_CenterAcross(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTextAlignmentType_CenterAcross(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkTextAlignmentType_CenterAcross(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


