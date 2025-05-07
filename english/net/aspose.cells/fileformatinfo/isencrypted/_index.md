---
title: FileFormatInfo.IsEncrypted
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Returns true if the document is encrypted and requires a password to open
type: docs
url: /net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Returns true if the document is encrypted and requires a password to open.

```csharp
public bool IsEncrypted { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(info.IsEncrypted, true);
[Test]
        public void Property_IsEncrypted()
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

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


