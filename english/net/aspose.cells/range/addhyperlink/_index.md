---
title: Range.AddHyperlink
second_title: Aspose.Cells for .NET API Reference
description: Range method. Adds a hyperlink to a specified cell or a range of cells
type: docs
url: /net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Adds a hyperlink to a specified cell or a range of cells.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

### Return Value

[`Hyperlink`](../../hyperlink/) object.

### Examples

```csharp
// Called: r.AddHyperlink("www.aspose.com", "www.aspose.com", "www.aspose.com");
public void Range_Method_AddHyperlink()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    Aspose.Cells.Range r = sheet.Cells.CreateRange("A1:A10");
    r.AddHyperlink("www.aspose.com", "www.aspose.com", "www.aspose.com");
    Assert.AreEqual("www.aspose.com", sheet.Hyperlinks[0].TextToDisplay);

}
```

### See Also

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


