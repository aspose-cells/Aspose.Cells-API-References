---
title: HtmlSaveOptions.ExportCellCoordinate
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Examples

```csharp
// Called: options.ExportCellCoordinate = true;
public void HtmlSaveOptions_Property_ExportCellCoordinate()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47922/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "Book1.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportCellCoordinate = true;
    wb.Save(savePath + "out.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


