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
// Called: LoadOptions loadOptions = new LoadOptions(FileFormatUtil.DetectFileFormat(filePath + &amp;quot;book.xlsm&amp;quot;).LoadFormat);
[Test]
        public void Property_LoadFormat()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET51595_&quot;;
            string savePath = CreateFolder(filePath);

            LoadOptions loadOptions = new LoadOptions(FileFormatUtil.DetectFileFormat(filePath + &quot;book.xlsm&quot;).LoadFormat);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            Workbook workbook = new Workbook(filePath + &quot;book.xlsm&quot;, loadOptions);

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            workbook.Save(savePath + &quot;out.pdf&quot;, saveOptions);

            Cell o10 = workbook.Worksheets[0].Cells[&quot;O10&quot;];
            Assert.AreEqual(o10.GetStyle().VerticalAlignment, TextAlignmentType.Center);

            Cell a7 = workbook.Worksheets[0].Cells[&quot;A7&quot;];
            Assert.AreEqual(a7.GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
        }
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


