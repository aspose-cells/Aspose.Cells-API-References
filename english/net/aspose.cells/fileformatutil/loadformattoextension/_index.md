---
title: FileFormatUtil.LoadFormatToExtension
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converts a load format enumerated value into a file extension
type: docs
url: /net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Converts a load format enumerated value into a file extension.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loaded file format. |

### Return Value

The returned extension is a lower-case string with a leading dot.

### Remarks

If it can not be converted, returns null.

### Examples

```csharp
// Called: suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003);
public void FileFormatUtil_Method_LoadFormatToExtension()
{
    //The annotated test code is currently not supported

    string suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto);
    Assert.AreEqual(null, suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv);
    Assert.AreEqual(".csv", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003);
    Assert.AreEqual(".xls", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx);
    Assert.AreEqual(".xlsx", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv);
    Assert.AreEqual(".txt", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.TabDelimited);
    Assert.AreEqual(".txt", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods);
    Assert.AreEqual(".ods", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.SpreadsheetML);
    Assert.AreEqual(".xml", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb);
    Assert.AreEqual(".xlsb", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Numbers);
    Assert.AreEqual(".numbers", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Fods);
    Assert.AreEqual(".fods", suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Image);
    Assert.AreEqual(null, suffix);

    suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Unknown);
    Assert.AreEqual(null, suffix);

            
    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Ots);
    //Assert.AreEqual(".ots", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xml);
    //Assert.AreEqual(".xml", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Epub);
    //Assert.AreEqual(".epub", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Azw3);
    //Assert.AreEqual(".azw3", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Html);
    //Assert.AreEqual(".html", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.MHtml);
    //Assert.AreEqual(".mhtml", suffix);


    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Sxc);
    //Assert.AreEqual(".sxc", suffix);

    //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Json);
    //Assert.AreEqual(".json", suffix);


}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


