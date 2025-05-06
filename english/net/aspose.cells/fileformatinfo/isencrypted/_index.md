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
// Called: Assert.IsFalse(Aspose.Cells.FileFormatUtil.DetectFileFormat(filePath).IsEncrypted);
[Test]
        public void Property_IsEncrypted()
        {
            string filePath = Constants.sourcePath + &quot;structure+protected.xls&quot;;
            Assert.IsFalse(Aspose.Cells.FileFormatUtil.DetectFileFormat(filePath).IsEncrypted);
        }
```

### See Also

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


