---
title: Cell.EmbeddedImage
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the embeddedn image in the cell
type: docs
url: /net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Gets and sets the embeddedn image in the cell.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["A1"].EmbeddedImage != null);
public void Cell_Property_EmbeddedImage()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsTrue(workbook.Worksheets[0].Cells["A1"].EmbeddedImage != null);
            
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


