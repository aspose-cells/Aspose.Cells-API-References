---
title: HtmlSaveOptions.ExportBogusRowData
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportBogusRowData = true;
public void HtmlSaveOptions_Property_ExportBogusRowData()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41169/";

    Workbook workbook = new Workbook(filePath + "sample2.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
    saveOptions.ExportActiveWorksheetOnly = true;
    saveOptions.ExportBogusRowData = false;
    workbook.Save(Constants.destPath + "example.html", saveOptions);
   string text = File.ReadAllText(Constants.destPath + "example.html");
    Assert.IsTrue(text.IndexOf("<![if supportMisalignedColumns]>") == -1);
    saveOptions.ExportBogusRowData = true;
    workbook.Save(Constants.destPath + "example.html", saveOptions);
    text = File.ReadAllText(Constants.destPath + "example.html");
    Assert.IsTrue(text.IndexOf("<![if supportMisalignedColumns]>") != -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


