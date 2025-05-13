---
title: HtmlSaveOptions.ExportFrameScriptsAndProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportFrameScriptsAndProperties = true;
public void HtmlSaveOptions_Property_ExportFrameScriptsAndProperties()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41458/";
    Workbook wb = new Workbook(filePath + "a.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportFrameScriptsAndProperties = true;

    string savePath = CreateFolder(filePath);
    wb.Save(savePath + "out.html", options);
    wb = new Workbook(savePath + "out.html");
    wb.Save(savePath + "out.xlsx");
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


