---
title: HtmlSaveOptions.CellNameAttribute
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specifies the attribute that indicates the CellName to be written. e.g. If the value is id then for cell A1 the output will betd idA1. The default value is null
type: docs
url: /net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```csharp
public string CellNameAttribute { get; set; }
```

### Examples

```csharp
// Called: saveOptions.CellNameAttribute = "id";
public void HtmlSaveOptions_Property_CellNameAttribute()
{
    Workbook workbook = new Workbook(Constants.HtmlPath + "example.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.CellNameAttribute = "id";
    saveOptions.ExportImagesAsBase64 = true;
    saveOptions.ExportActiveWorksheetOnly = true;
    workbook.Save(_destFilesPath + "example.html", saveOptions);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    string pattern = @"<td\s+id='A23'\s+[^>]*style='[^']*background:*#FFFFFF;[^']*'[^>]*>"; 
    Assert.IsTrue(Regex.IsMatch(text, pattern));
    pattern = @"<td\s+id='B27'\s+[^>]*style='[^']*background:*#FFFFFF;[^']*'[^>]*>";
    Assert.IsTrue(Regex.IsMatch(text, pattern));
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


