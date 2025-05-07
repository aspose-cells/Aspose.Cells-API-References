---
title: HtmlSaveOptions.ExportActiveWorksheetOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file If false then the whole workbook will be exported to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Examples

```csharp
// Called: opt.ExportActiveWorksheetOnly = true;
[Test]
        public void Property_ExportActiveWorksheetOnly()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSJAVA-45714.xls");
            wb.Worksheets.ActiveSheetIndex = 0;
            HtmlSaveOptions opt = new HtmlSaveOptions();
            opt.ExportActiveWorksheetOnly = true;
            wb.Save(_destFilesPath + "CELLSJAVA-45714.html", opt);
            string text = File.ReadAllText(wb.FileName);
            Assert.IsTrue(text.IndexOf("<font class=\"font3\" style=\"text-decoration: none;\">江苏果下科技有限公司<span style='display:none'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></font><font class=\"font4\" style=\"text-decoration: none;\"><span style='display:none'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></font>") > 0);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


