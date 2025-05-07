---
title: HtmlSaveOptions.ExportHiddenWorksheet
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating if exporting the hidden worksheet content.The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indicating if exporting the hidden worksheet content.The default value is true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportHiddenWorksheet = false;
[Test]
        public void Property_ExportHiddenWorksheet()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42465/";
            Workbook workbook = new Workbook(filePath + "input.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportHiddenWorksheet = false;
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.CellCssPrefix = "prefix123";
            saveOptions.TableCssId = "asdf";
            workbook.Save(CreateFolder(filePath) + "out.html", saveOptions);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


