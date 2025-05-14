---
title: HtmlSaveOptions.ExportArea
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```csharp
public CellArea ExportArea { get; set; }
```

### Examples

```csharp
// Called: options.ExportArea = CellArea.CreateCellArea("B5", "E7");
public void HtmlSaveOptions_Property_ExportArea()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43018/";
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportPrintAreaOnly = true;
    options.ExportArea = CellArea.CreateCellArea("B5", "E7");
    Workbook wb = new Workbook(filePath + "a.xlsx");
    wb.Save(CreateFolder(filePath) + "out.html", options);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


