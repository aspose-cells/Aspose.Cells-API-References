---
title: Cells.Style
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets and sets the default style of the worksheet
type: docs
url: /net/aspose.cells/cells/style/
---
## Cells.Style property

Gets and sets the default style of the worksheet.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(Color.Black.ToArgb() & 0xFFFFFF, workbook.Worksheets[0].Cells.Style.Font.Color.ToArgb() & 0xFFFFFF);
[Test]
        public void Property_Style()
        {
            Workbook workbook = new Workbook();
            Assert.AreEqual(Color.Black.ToArgb() & 0xFFFFFF, workbook.Worksheets[0].Cells.Style.Font.Color.ToArgb() & 0xFFFFFF);
        }
```

### See Also

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


