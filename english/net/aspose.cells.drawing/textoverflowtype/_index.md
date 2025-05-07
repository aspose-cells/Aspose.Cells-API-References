---
title: Enum TextOverflowType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.TextOverflowType enum. Represents the way the text vertical or horizontal overflow
type: docs
url: /net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Represents the way the text vertical or horizontal overflow.

```csharp
public enum TextOverflowType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Clip | `0` | Pay attention to top and bottom barriers. Provide no indication that there is text which is not visible. |
| Ellipsis | `1` | Pay attention to top and bottom barriers. Use an ellipsis to denote that there is text which is not visible. Only for vertical overflow. |
| Overflow | `2` | Overflow the text and pay no attention to top and bottom barriers. |

### Examples

```csharp
// Called: Assert.AreEqual(TextOverflowType.Overflow, shape.TextVerticalOverflow );
[Test]
        public void Type_TextOverflowType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet53180.xlsx");
            workbook.Save(Constants.destPath + "CellsNet53180.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet53180.xls");
            Shape shape = workbook.Worksheets[0].Shapes[1];
            Assert.AreEqual(TextOverflowType.Overflow, shape.TextVerticalOverflow );
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


