---
title: OleObject.DisplayAsIcon
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. True if the specified object is displayed as an icon and the image will not be auto changed
type: docs
url: /net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True if the specified object is displayed as an icon and the image will not be auto changed.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Examples

```csharp
// Called: newEmbeddedObject.DisplayAsIcon = false;
public void OleObject_Property_DisplayAsIcon()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45834.Xls");
    workbook.Worksheets[0].OleObjects.RemoveAt(0);
    workbook.Worksheets[0].Pictures.RemoveAt(0);

    //Add pdf
    byte[] iconData = File.ReadAllBytes(Constants.sourcePath + @"CellsNet45834.Emf");
    int newOleNumber = workbook.Worksheets[0].OleObjects.Add(10, 10, 533, 533, iconData);
    OleObject newEmbeddedObject = workbook.Worksheets[0].OleObjects[newOleNumber];
    newEmbeddedObject.ObjectData = File.ReadAllBytes(Constants.sourcePath + @"example.pdf");
    newEmbeddedObject.ProgID = "AcroExch.Document.DC";
    newEmbeddedObject.DisplayAsIcon = false;
    newEmbeddedObject.FileFormatType = (FileFormatType)13; // pdf format.
    Util.SaveManCheck(workbook, "Shape", "example.xls");
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


