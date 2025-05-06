---
title: Class CellRichValue
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellRichValue class. Represents rich value of the cell
type: docs
url: /net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Represents rich value of the cell.

```csharp
public abstract class CellRichValue
```

## Properties

| Name | Description |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Gets the alt text associated with the image. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Gets the error value type of the cell. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Gets the image data of the cell. |

### Examples

```csharp
// Called: CellRichValue c = w.Worksheets[0].Cells[&amp;quot;A1&amp;quot;].GetRichValue();
[Test]
        public void Type_CellRichValue()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET57143.xlsx&quot;);
            Workbook w = new Workbook();
            w.Worksheets[0].Copy(wb.Worksheets[0]);
            CellRichValue c = w.Worksheets[0].Cells[&quot;A1&quot;].GetRichValue();
            Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
            w.Save(Constants.destPath + &quot;CELLSNET57143.xlsx&quot;);
            w = new Workbook(Constants.destPath + &quot;CELLSNET57143.xlsx&quot;);
            c = w.Worksheets[0].Cells[&quot;A1&quot;].GetRichValue();
            Assert.AreEqual(ErrorCellValueType.Spill, c.ErrorValue);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


