---
title: FileFormatInfo.FileFormatType
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Gets the detected file format
type: docs
url: /net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

Gets the detected file format.

```csharp
public FileFormatType FileFormatType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(info.FileFormatType, FileFormatType.Excel97To2003);
public void FileFormatInfo_Property_FileFormatType()
{
    string excelFileNameAndPath = Constants.sourcePath + "no+macros+plus+ext+password.xls";
    FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFileNameAndPath);
    Assert.AreEqual(info.IsEncrypted,true);
    Assert.AreEqual(info.FileFormatType, FileFormatType.Excel97To2003);

    string file = Constants.sourcePath + "TestWorkbook/Book3.xlsx";
    info = FileFormatUtil.DetectFileFormat(file);
    Assert.AreEqual(info.IsEncrypted, true);
    Assert.AreEqual(info.FileFormatType, FileFormatType.Ooxml);
}
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


