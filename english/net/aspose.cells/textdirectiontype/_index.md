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
// Called: testAreEqual(TextDirectionType.Context, cells[0, 0].GetStyle().TextDirection, caseName);
private void Type_TextDirectionType(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(TextDirectionType.Context, cells[0, 0].GetStyle().TextDirection, caseName);
            testAreEqual(TextDirectionType.LeftToRight, cells[1, 0].GetStyle().TextDirection, caseName);
            testAreEqual(TextDirectionType.RightToLeft, cells[2, 0].GetStyle().TextDirection, caseName);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


