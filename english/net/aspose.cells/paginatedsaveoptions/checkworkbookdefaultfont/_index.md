---
title: PaginatedSaveOptions.CheckWorkbookDefaultFont
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set this to true to try to use workbooks default font to show these characters first
type: docs
url: /net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Remarks

Default is true.

### Examples

```csharp
// Called: saveOptions.CheckWorkbookDefaultFont = false;
[Test]
        public void Property_CheckWorkbookDefaultFont()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47688/";
            string savePath = CreateFolder(filePath);

            var fileName = filePath + @"f.html";
            var output2 = savePath + @"out.pdf";
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            Workbook wb = new Workbook(fileName, loadOptions);
            Worksheet worksheet = wb.Worksheets[0];
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            worksheet.AutoFitRows(options);
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsPercentScale = true;
            pageSetup.Zoom = 70;
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            wb.Save(output2, saveOptions);
            wb.Save(savePath + "out.xlsx");

        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


