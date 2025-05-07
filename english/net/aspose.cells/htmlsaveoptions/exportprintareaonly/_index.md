---
title: HtmlSaveOptions.ExportPrintAreaOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the print area to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indicates if only exporting the print area to html file. The default value is false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Examples

```csharp
// Called: options.ExportPrintAreaOnly = true;
[Test]
        public void Property_ExportPrintAreaOnly()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET46465/";


            String namedRng = "Line_Chart_Data";

            Workbook wb = new Workbook(filePath + "InlineCharts.xlsx");

            Name name = wb.Worksheets.Names[namedRng];
            Worksheet sheet = name.GetRange().Worksheet;

            wb.Worksheets.ActiveSheetIndex = sheet.Index;

            Console.WriteLine(sheet.Name);
            Console.WriteLine(name.GetRange().Address);
            sheet.PageSetup.PrintArea = name.GetRange().Address;

            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.ExportActiveWorksheetOnly = true;
            options.ExportPrintAreaOnly = true;

            wb.Save(CreateFolder(filePath) + "out.xlsx");
            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


