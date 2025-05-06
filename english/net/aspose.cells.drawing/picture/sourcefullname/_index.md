---
title: Picture.SourceFullName
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets or sets the path and name of the source file for the linked image
type: docs
url: /net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Gets or sets the path and name of the source file for the linked image.

```csharp
public string SourceFullName { get; set; }
```

### Remarks

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### Examples

```csharp
// Called: Assert.IsTrue(!string.IsNullOrEmpty(picture.SourceFullName));
[Test]
        public void Property_SourceFullName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47362.xlsx&quot;);
            Picture picture = workbook.Worksheets[0].Pictures[0];
            byte[] data = picture.Data;//exception 
            if (picture.IsLink)
            {

                Assert.IsTrue(!string.IsNullOrEmpty(picture.SourceFullName));
                Assert.IsTrue(data == null);
            }
        }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


