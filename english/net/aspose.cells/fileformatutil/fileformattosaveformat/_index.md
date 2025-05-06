---
title: FileFormatUtil.FileFormatToSaveFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converting file format to save format
type: docs
url: /net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Converting file format to save format.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | FileFormatType | The file format type. |

### Examples

```csharp
// Called: SaveFormat saveformat = FileFormatUtil.FileFormatToSaveFormat(format);
[Test]
       
        public void Method_FileFormatType_()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45637.xls&quot;);
            FileFormatType format = book.FileFormat;
            SaveFormat saveformat = FileFormatUtil.FileFormatToSaveFormat(format);
            String formatStr = FileFormatUtil.SaveFormatToExtension(saveformat);
            Assert.IsFalse(string.IsNullOrEmpty(formatStr));

            book = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45637.ots&quot;);
            format = book.FileFormat;
            saveformat = FileFormatUtil.FileFormatToSaveFormat(format);
            formatStr = FileFormatUtil.SaveFormatToExtension(saveformat);
            Assert.IsFalse(string.IsNullOrEmpty(formatStr));
            Assert.AreNotEqual(-1, formatStr.IndexOf(&quot;ots&quot;));
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


