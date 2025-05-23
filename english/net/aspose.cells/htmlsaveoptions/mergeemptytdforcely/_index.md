---
title: HtmlSaveOptions.MergeEmptyTdForcely
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Examples

```csharp
// Called: options.MergeEmptyTdForcely = true;
public void HtmlSaveOptions_Property_MergeEmptyTdForcely()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47672/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "sample.xlsm");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.MergeEmptyTdForcely = true;
    wb.Save(savePath + "out.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


