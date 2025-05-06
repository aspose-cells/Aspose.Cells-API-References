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
// Called: Assert.IsTrue(oleObject.ObjectSourceFullName != null);
[Test]
        public void Property_ObjectSourceFullName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46876.xls&quot;);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[1];
            Assert.IsTrue(oleObject.ObjectSourceFullName != null);
            workbook.Save(Constants.destPath + &quot;CellsNet46876.xls&quot;);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


