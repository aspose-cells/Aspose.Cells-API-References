---
title: OleObject.ObjectSourceFullName
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Returns the source full name of the source file for the linked OLE object
type: docs
url: /net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Returns the source full name of the source file for the linked OLE object.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Remarks

Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..

### Examples

```csharp
// Called: Assert.AreEqual(SourceBook1.Worksheets[SourceBook1.Worksheets.Count - 1].OleObjects[0].ObjectSourceFullName,null);
public void OleObject_Property_ObjectSourceFullName()
{
    Workbook SourceBook1 = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook SourceBook2 = new Workbook(Constants.sourcePath + "example.xlsx");
    SourceBook1.Combine(SourceBook2);
    SourceBook1.Save(Constants.destPath + "example.xlsx");
    SourceBook1 = new Workbook(Constants.destPath + "example.xlsx");
    SourceBook1.Combine(SourceBook2);
    Assert.AreEqual(SourceBook1.Worksheets[SourceBook1.Worksheets.Count - 1].OleObjects[0].ObjectSourceFullName,null);
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


