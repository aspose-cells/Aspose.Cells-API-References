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
// Called: Assert.IsTrue(wb.Worksheets[0].OleObjects[0].ObjectSourceFullName.EndsWith("申請進入.txt"));
[Test]
        public void Property_ObjectSourceFullName()
        {
            Workbook wb = new Workbook();
            ShapeCollection shapes = wb.Worksheets[0].Shapes;
            shapes.AddOleObject(0, 0, 0, 0, 100, 100, File.ReadAllBytes(Constants.sourcePath + "image1.png"));
            OleObject oleObject = (OleObject)shapes[0];
            oleObject.ObjectData = File.ReadAllBytes(Constants.sourcePath + "申請進入.txt");
            oleObject.ObjectSourceFullName = Constants.sourcePath + "申請進入.txt";

            wb.Save(Constants.destPath + "CELLSJAVA42521.xlsx");
            wb = new Workbook(Constants.destPath + "CELLSJAVA42521.xlsx");
            Assert.IsTrue(wb.Worksheets[0].OleObjects[0].ObjectSourceFullName.EndsWith("申請進入.txt"));

        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


