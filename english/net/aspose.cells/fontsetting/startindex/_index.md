---
title: FontSetting.StartIndex
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Gets the start index of the characters
type: docs
url: /net/aspose.cells/fontsetting/startindex/
---
## FontSetting.StartIndex property

Gets the start index of the characters.

```csharp
public int StartIndex { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Example 1.1", cell.StringValue.Substring(fs.StartIndex, fs.Length));
public void FontSetting_Property_StartIndex()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];

    string value = "<b>Example Test</b><div><ul><li>Example 1<ul><li><span style=\"font-size:1.16rem;text-transform:inherit\">Example 1.1</span> <ul><li><span style=\"font-size:1.16rem;text-transform:inherit\">Example 1.1.1</span> </li></ul></li></ul></li><li>Example 2<ul><li>Example 2.1 </li><li>Example 2.2</li></ul></li></ul></div>";
    Cell cell = worksheet.Cells[1, 1];
    cell.HtmlString = value;
    FontSetting[] fontSettings = cell.GetCharacters();
    FontSetting fs = fontSettings[5];
    Assert.AreEqual(11.6, fs.Font.DoubleSize);
    Assert.AreEqual("Example 1.1", cell.StringValue.Substring(fs.StartIndex, fs.Length));
}
```

### See Also

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


