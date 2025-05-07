---
title: FileFormatInfo.LoadFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Gets the detected load format
type: docs
url: /net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Gets the detected load format.

```csharp
public LoadFormat LoadFormat { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(LoadFormat.Xlsx, info.LoadFormat);
[Test]
        public void Property_LoadFormat()
        {
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CELLSNET55355.xlsx");
            Assert.AreEqual(LoadFormat.Xlsx, info.LoadFormat);
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
          Assert.AreEqual(SaveFormat.Xlsx,saveFormat);
           Assert.AreEqual(LoadFormat.Xlsx, loadFormat);
        }
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


