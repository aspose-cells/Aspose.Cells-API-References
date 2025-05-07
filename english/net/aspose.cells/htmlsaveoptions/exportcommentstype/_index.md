---
title: HtmlSaveOptions.ExportCommentsType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Represents type of exporting comments to html files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Represents type of exporting comments to html files.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
[Test]
        public void Property_ExportCommentsType()
        {
            Workbook workbook = new Workbook(Constants.HtmlSourcePath + "CELLSNET51665.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            workbook.Save(Constants.HtmlDestPath + "CELLSNET51665.html", saveOptions);
            string text = File.ReadAllText(Constants.HtmlDestPath + "CELLSNET51665.html");
            Assert.IsTrue(text.IndexOf("function DisplayComment(id") != -1);
        }
```

### See Also

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


