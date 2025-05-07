---
title: HtmlSaveOptions.HtmlCrossStringType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if a crosscell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default so for crosscell strings there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html filessetting the value to Cross would be several times faster than setting it to Default or Fit2Cell
type: docs
url: /net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.HtmlCrossStringType = HtmlCrossType.Cross;
[Test, Description("HtmlSaveOptions.DisplayHTMLCrossString property need be checked by Manual")]
        public void Property_HtmlCrossStringType()
        {
            string file = Constants.sourcePath + "TestWorkbook\\savetest.xls";
            Workbook workbook = new Workbook(file);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.HtmlCrossStringType = HtmlCrossType.Cross;
            workbook.Save(Constants.checkPath + "HtmlSaveOptions_DisplayHTMLCrossString_001.html", saveOptions);
        }
```

### See Also

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


