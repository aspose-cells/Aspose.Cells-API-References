---
title: HtmlSaveOptions.HtmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions constructor. Creates options for saving html file
type: docs
url: /net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Creates options for saving html file.

```csharp
public HtmlSaveOptions()
```

### Examples

```csharp
// Called: HtmlSaveOptions saveOptions = new HtmlSaveOptions();
public void HtmlSaveOptions_Constructor()
{
    //chrome  does not support font size <12
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportActiveWorksheetOnly = (true);
    workbook.Save(_destFilesPath + "example.html", saveOptions);
    string str = File.ReadAllText(_destFilesPath + "example.html");
    // Assert.IsTrue(str.IndexOf("var spans=[1,1,1,1,1,1,1,1,1,1];") != -1);
    //  Assert.IsTrue(str.IndexOf("var spans=[1,1,1,1,1,1,1,1,1,1];") != -1);
    Assert.IsTrue(str.IndexOf("overflow:hidden;line-height:0;'>hidden</td>") > -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving htm file.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Html or MHtml, otherwise the saved format will be set as Html automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


