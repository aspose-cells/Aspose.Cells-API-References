---
title: HtmlSaveOptions.ExportGridLines
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting the gridlines.The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Indicating whether exporting the gridlines.The default value is false.

```csharp
public bool ExportGridLines { get; set; }
```

### Examples

```csharp
// Called: var saveOptions2 = new HtmlSaveOptions { ExportImagesAsBase64 = true, ExportActiveWorksheetOnly = true, ExportGridLines = true };
[Test]
        public void Property_ExportGridLines()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45807/&quot;;

            //same workbook with a second blank worksheet, this only works if the ExportActiveWorksheetOnly property is set to false 
            var workbookStream2 = new FileStream(filePath + &quot;gridlines_off_2worksheets.xls&quot;, FileMode.Open);
            var workbook2 = new Workbook(workbookStream2);
            var saveOptions2 = new HtmlSaveOptions { ExportImagesAsBase64 = true, ExportActiveWorksheetOnly = true, ExportGridLines = true };
            workbook2.CalculateFormula();
            workbook2.Worksheets[workbook2.Worksheets.ActiveSheetIndex].IsGridlinesVisible = true;
            workbook2.Save(CreateFolder(filePath) + @&quot;out.html&quot;, saveOptions2);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


