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
// Called: Assert.AreEqual(64,wb.Worksheets[0].Cells.StandardWidthPixels);
[Test]
        public void Property_StandardWidthPixels()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Cellsnet52338.ods&quot;);
           Assert.AreEqual(64,wb.Worksheets[0].Cells.StandardWidthPixels);
            wb.Save(Constants.destPath + &quot;Cellsnet52338.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


