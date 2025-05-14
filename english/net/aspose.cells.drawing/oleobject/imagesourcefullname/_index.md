---
title: OleObject.ImageSourceFullName
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets or sets the path and name of the source file for the linked image
type: docs
url: /net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Gets or sets the path and name of the source file for the linked image.

```csharp
public string ImageSourceFullName { get; set; }
```

### Remarks

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### Examples

```csharp
// Called: obj.ImageSourceFullName = null;
public void OleObject_Property_ImageSourceFullName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet worksheet = workbook.Worksheets[0];
    OleObject oleObj = worksheet.OleObjects[0];

    byte[] pdfBytes = File.ReadAllBytes(Constants.sourcePath + "example.pdf");

    OleObject obj = worksheet.OleObjects[0];

    obj.DisplayAsIcon = false;
    obj.FileFormatType = FileFormatType.Pdf;
    obj.ImageSourceFullName = null;
    obj.IsAutoSize = false;
    obj.IsLink = false;
    obj.ObjectData = pdfBytes;
    obj.ObjectSourceFullName = null;
    obj.ProgID = "Acrobat Document";

    Util.SaveManCheck(workbook, "Shape", "example.xls");

}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


