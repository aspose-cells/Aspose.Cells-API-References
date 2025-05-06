---
title: OleObject.ImageData
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Represents image of ole object as byte array
type: docs
url: /net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Represents image of ole object as byte array.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(oleObject.ImageData != null);
[Test]
        public void Property_ImageData()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSAPP1504.xls&quot;);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[0];
            Assert.IsTrue(oleObject.ImageData != null);
            Assert.IsFalse(oleObject.IsHidden);
            workbook.Save(Constants.destPath + &quot;CELLSAPP1504.xls&quot;);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


