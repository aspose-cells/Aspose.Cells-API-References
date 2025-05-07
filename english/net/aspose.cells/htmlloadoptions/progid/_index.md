---
title: HtmlLoadOptions.ProgId
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Gets the program id of creating the file. Only for MHT files
type: docs
url: /net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Gets the program id of creating the file. Only for MHT files.

```csharp
public string ProgId { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(options.ProgId, "Word.Document");
[Test]
        public void Property_ProgId()
        {
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            Workbook workbook = new Workbook(Constants.MhtmlPath + "CellsNet46544excel.mht", options);
            Assert.AreEqual(options.ProgId, "Excel.Sheet");
            options = new HtmlLoadOptions(LoadFormat.MHtml);
#if !LINUX_TEST
            workbook = new Workbook(Constants.MhtmlPath + "CellsNet46544word.mht", options);
            Assert.AreEqual(options.ProgId, "Word.Document");
#endif
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


