---
title: Cells.StandardWidthPixels
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default column width in the worksheet in unit of pixels
type: docs
url: /net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Gets or sets the default column width in the worksheet, in unit of pixels.

```csharp
public int StandardWidthPixels { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(104,wb.Worksheets[0].Cells.StandardWidthPixels);
[Test]
        public void Property_StandardWidthPixels()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET49922.xls");
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(104,wb.Worksheets[0].Cells.StandardWidthPixels);
            Assert.AreEqual(12.375, wb.Worksheets[0].Cells.StandardWidth);
            Assert.AreEqual(14.25, wb.Worksheets[0].Cells.StandardHeight);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


