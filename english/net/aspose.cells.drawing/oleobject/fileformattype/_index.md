---
title: OleObject.FileFormatType
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets and sets the file type of the embedded ole object data
type: docs
url: /net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Gets and sets the file type of the embedded ole object data

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FileFormatType.Pptm, workbook.Worksheets[1].OleObjects[0].FileFormatType);
[Test]
        public void Property_FileFormatType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46697.xlsm");
            Assert.AreEqual(FileFormatType.Pptm, workbook.Worksheets[1].OleObjects[0].FileFormatType);
            workbook.Save(Constants.destPath + "CellsNet46697.xls");
        }
```

### See Also

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


