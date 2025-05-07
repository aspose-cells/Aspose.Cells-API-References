---
title: MsoFillFormat.ImageData
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets and sets the Texture and Picture fill data
type: docs
url: /net/aspose.cells.drawing/msofillformat/imagedata/
---
## MsoFillFormat.ImageData property

Gets and sets the Texture and Picture fill data.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Shapes[0].FillFormat.ImageData != null, true);
[Test]
        public void Property_ImageData()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44178.xlsx");
            workbook.Save(Constants.destPath + "CellsNet44178.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet44178.ods");
            Assert.AreEqual(workbook.Worksheets[0].Shapes[0].FillFormat.ImageData != null, true);
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


