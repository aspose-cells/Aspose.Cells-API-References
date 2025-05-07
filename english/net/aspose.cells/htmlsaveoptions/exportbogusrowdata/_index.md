---
title: HtmlSaveOptions.ExportBogusRowData
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Examples

```csharp
// Called: options.ExportBogusRowData = false;
[Test]
        public void Property_ExportBogusRowData()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42471/";

            Workbook workbook = new Workbook(filePath + "input.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            Worksheet sheet = workbook.Worksheets["Entry points"];
            workbook.Worksheets.ActiveSheetIndex = sheet.Index;
            options.ExportActiveWorksheetOnly = true;
            options.ExportBogusRowData = false;
            options.ExportFrameScriptsAndProperties = false;
            options.ExcludeUnusedStyles = true;
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetProperties = false;
            workbook.Save(CreateFolder(filePath) + "out.html", options);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


