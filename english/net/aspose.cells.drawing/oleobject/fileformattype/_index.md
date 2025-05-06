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
// Called: Assert.AreEqual(sheet.OleObjects[1].FileFormatType, FileFormatType.Doc);
[Test]
        public void Property_FileFormatType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +&quot;Embedded.xls&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;DOC + DOCX&quot;];
            Assert.AreEqual(sheet.OleObjects[0].FileFormatType, FileFormatType.Docx);
            Assert.AreEqual(sheet.OleObjects[1].FileFormatType, FileFormatType.Doc);
            workbook.Save(Constants.destPath + &quot;dest.xls&quot;);
        }
```

### See Also

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


