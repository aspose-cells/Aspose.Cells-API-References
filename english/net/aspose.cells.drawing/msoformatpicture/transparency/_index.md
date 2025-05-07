---
title: MsoFormatPicture.Transparency
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0.5, workbook.Worksheets[0].Pictures[0].FormatPicture.Transparency);
[Test]
        public void Property_Transparency()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet49052.xlsx");
            Assert.AreEqual(0.5, workbook.Worksheets[0].Pictures[0].FormatPicture.Transparency);
            Assert.AreEqual(0.69, workbook.Worksheets[0].Pictures[1].FormatPicture.Transparency);
            workbook.Save(Constants.destPath + "CellsNet49052.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet49052.xlsx");
            Assert.AreEqual(0.5, workbook.Worksheets[0].Pictures[0].FormatPicture.Transparency);
            Assert.AreEqual(0.69, workbook.Worksheets[0].Pictures[1].FormatPicture.Transparency);
        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


