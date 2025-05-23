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
// Called: options.HtmlCrossStringType = HtmlCrossType.MSExport;
public void Cells_Type_HtmlCrossType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42417And42418And42419/";
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.HtmlCrossStringType = HtmlCrossType.MSExport;
    Workbook wb = new Workbook(filePath + "RP_xls_1.xls");
    wb.Save(CreateFolder(filePath) + "out.html", options);
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


