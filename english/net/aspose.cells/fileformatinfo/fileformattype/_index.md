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
// Called: Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.odp").FileFormatType,FileFormatType.Odp);
[Test]
        public void Property_FileFormatType()
        {
#if NETCOREAPP2_0
            CellsHelper.InitForDotNetCore();
#endif
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.odp").FileFormatType,FileFormatType.Odp);
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.odf").FileFormatType, FileFormatType.Odf);
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.odg").FileFormatType, FileFormatType.Odg);
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.odt").FileFormatType, FileFormatType.Odt);
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CellsJava41714.ods").FileFormatType, FileFormatType.Ods);
        }
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


