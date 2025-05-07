---
title: Enum TextDirectionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.TextDirectionType enum. Represents the direction of the text flow for this paragraph
type: docs
url: /net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Represents the direction of the text flow for this paragraph.

```csharp
public enum TextDirectionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Examples

```csharp
// Called: style.TextDirection = TextDirectionType.Context;
[Test]
        public void Type_TextDirectionType()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[1, 1].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells[1, 1].SetStyle(style);

            checkTextDirectionType_Context(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTextDirectionType_Context(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTextDirectionType_Context(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkTextDirectionType_Context(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


