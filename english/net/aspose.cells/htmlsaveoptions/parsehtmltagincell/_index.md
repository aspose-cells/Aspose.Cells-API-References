---
title: HtmlSaveOptions.ParseHtmlTagInCell
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether html tagsuch as div/div in cell should be parsed as cell value or preserved as it is. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Examples

```csharp
// Called: ParseHtmlTagInCell = true,
private Aspose.Cells.HtmlSaveOptions Property_ParseHtmlTagInCell(Aspose.Cells.Workbook tmpWb)
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


