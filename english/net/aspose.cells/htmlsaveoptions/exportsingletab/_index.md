---
title: HtmlSaveOptions.ExportSingleTab
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Examples

```csharp
// Called: options.ExportSingleTab = true;
[Test]
        public void Property_ExportSingleTab()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET46479/";


            Workbook wb = new Workbook(filePath + "a.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportSingleTab = true;
            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


