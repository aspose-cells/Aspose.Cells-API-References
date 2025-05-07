---
title: Enum HtmlCrossType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HtmlCrossType enum. Represents five types of html cross string
type: docs
url: /net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Represents five types of html cross string.

```csharp
public enum HtmlCrossType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated |
| MSExport | `1` | Display the string like MS Excel exporting html. |
| Cross | `2` | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | `3` | Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | `4` | Only displaying the string within the width of cell. |

### Examples

```csharp
// Called: htmlSaveOptions.HtmlCrossStringType = HtmlCrossType.FitToCell;
[Test]
        public void Type_HtmlCrossType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42853/";

            Workbook workbook = new Workbook(filePath + "view_qldtl_Admin.xlsx");
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.DisableDownlevelRevealedComments = true;
            htmlSaveOptions.ExcludeUnusedStyles = true;
            htmlSaveOptions.ExportActiveWorksheetOnly = true;
            htmlSaveOptions.ExportDocumentProperties = false;
            htmlSaveOptions.ExportFrameScriptsAndProperties = false;
            htmlSaveOptions.ExportImagesAsBase64 = false;
            htmlSaveOptions.ExportPrintAreaOnly = true;
            htmlSaveOptions.ExportSimilarBorderStyle = true;
            htmlSaveOptions.ExportWorkbookProperties = false;
            htmlSaveOptions.ExportWorksheetCSSSeparately = false;
            htmlSaveOptions.ExportWorksheetProperties = false;
            htmlSaveOptions.ParseHtmlTagInCell = true;
            htmlSaveOptions.HtmlCrossStringType = HtmlCrossType.FitToCell;

            DateTime start = DateTime.Now;

            workbook.Save(CreateFolder(filePath) + "out.html", htmlSaveOptions);

            Assert.Less(DateTime.Now.Subtract(start).Seconds, 30);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


