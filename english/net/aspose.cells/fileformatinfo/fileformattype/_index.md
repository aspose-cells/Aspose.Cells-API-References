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
// Called: Assert.AreEqual(finf.FileFormatType, FileFormatType.Xlam);
[Test]
        public void Property_FileFormatType()
        {
#if NETCOREAPP2_0
            CellsHelper.InitForDotNetCore();
#endif
            FileFormatInfo finf = FileFormatUtil.DetectFileFormat(Constants.sourcePath + &quot;CELLSJAVA42594.xlam&quot;); 
            Assert.AreEqual(finf.FileFormatType, FileFormatType.Xlam);
        }
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


