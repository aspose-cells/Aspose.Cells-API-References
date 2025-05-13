---
title: Picture.IsLink
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Returns true if the picture is linked to a file
type: docs
url: /net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Returns true if the picture is linked to a file.

```csharp
public bool IsLink { get; set; }
```

### Examples

```csharp
// Called: if (picture.IsLink)
public void Picture_Property_IsLink()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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


