---
title: HtmlLoadOptions.HtmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions()
```

### Examples

```csharp
// Called: HtmlLoadOptions loadOptions = new HtmlLoadOptions();
public void HtmlLoadOptions_Constructor()
{
    HtmlLoadOptions loadOptions = new HtmlLoadOptions();
    loadOptions.SupportDivTag = true;
    Workbook wb = new Workbook(Constants.HtmlPath + "example.html", loadOptions);
    Assert.AreEqual("Internal", wb.Worksheets[0].Cells["B1"].StringValue);
    Assert.AreEqual("Internal", wb.Worksheets[0].Cells["B1"].StringValue);
    Assert.AreEqual("testingggg", wb.Worksheets[0].Cells["B3"].StringValue);
    Assert.AreEqual("testinggggerertwrt", wb.Worksheets[0].Cells["B4"].StringValue);
}
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


