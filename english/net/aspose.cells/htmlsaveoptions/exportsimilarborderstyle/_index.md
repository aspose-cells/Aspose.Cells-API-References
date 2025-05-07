---
title: HtmlSaveOptions.ExportSimilarBorderStyle
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel please keep the default value. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Examples

```csharp
// Called: options.ExportSimilarBorderStyle = true;
public void Property_ExportSimilarBorderStyle()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42552/";
            Workbook wb = new Workbook(filePath + "ATLAS Sports 入会礼品样品费用借款单 (1).xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportSimilarBorderStyle = true;
            wb.Save(_destFilesPath + "JAVA42552.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


