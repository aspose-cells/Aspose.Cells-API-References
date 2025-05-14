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
// Called: ExportGridLines = tmpWb.Worksheets[0].IsGridlinesVisible == true ? true : false,
private Aspose.Cells.HtmlSaveOptions HtmlSaveOptions_Property_ExportGridLines(Aspose.Cells.Workbook tmpWb)
        {
            return new Aspose.Cells.HtmlSaveOptions
            {
                ExportGridLines = tmpWb.Worksheets[0].IsGridlinesVisible == true ? true : false,
                ExportActiveWorksheetOnly = true,
                ParseHtmlTagInCell = true,
                ExcludeUnusedStyles = true,

                HtmlCrossStringType = HtmlCrossType.MSExport,
            };

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


