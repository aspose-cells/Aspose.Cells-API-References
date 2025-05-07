---
title: HtmlSaveOptions.IsExportComments
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if exporting comments when saving file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indicates if exporting comments when saving file to html, the default value is false.

```csharp
public bool IsExportComments { get; set; }
```

### Examples

```csharp
// Called: saveOptions.IsExportComments = true;
[Test]
        public void Property_IsExportComments()
        {
            Workbook wb = new Aspose.Cells.Workbook(Constants.HtmlPath + "CELLSNET-55893.xlsx");
            wb.Worksheets.ActiveSheetIndex = 1;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportActiveWorksheetOnly = true; 
            saveOptions.IsExportComments = true;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintSheetEnd;
            wb.Save(_destFilesPath + "CELLSNET-55893.html", saveOptions);
            string text = File.ReadAllText(_destFilesPath + "CELLSNET-55893.html");
            int n1 = text.IndexOf("<div id = 'Comment_1_1' style='text-align:left;'");
            int n2 = text.IndexOf("<div id = 'Comment_1_2' style='text-align:left;'");
            int n3 = text.IndexOf("<div id = 'Comment_1_3' style='text-align:left;'");
            int n4 = text.IndexOf("<div id = 'Comment_1_4' style='text-align:left;'");
            Assert.IsTrue(-1 < n1 && n1 < n2 && n2 < n3 && n3 < n4);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


