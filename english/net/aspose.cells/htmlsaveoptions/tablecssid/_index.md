---
title: HtmlSaveOptions.TableCssId
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets and sets the prefix of the type css name such as trcoltd and so on they are contained in the table element which has the specific TableCssId attribute. The default value is 
type: docs
url: /net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```csharp
public string TableCssId { get; set; }
```

### Examples

```csharp
// Called: saveOptions.TableCssId = "asdf";
public void HtmlSaveOptions_Property_TableCssId()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42465/";
    Workbook workbook = new Workbook(filePath + "input.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
    saveOptions.ExportHiddenWorksheet = false;
    saveOptions.ExportActiveWorksheetOnly = true;
    saveOptions.CellCssPrefix = "prefix123";
    saveOptions.TableCssId = "asdf";
    workbook.Save(CreateFolder(filePath) + "out.html", saveOptions);

}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


