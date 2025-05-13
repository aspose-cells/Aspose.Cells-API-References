---
title: Cell.GetCharacters
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns all Characters objects that represents a range of characters within the cell text
type: docs
url: /net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters()
```

### Return Value

All Characters objects

### Examples

```csharp
// Called: fonts = worksheet.Cells["A1"].GetCharacters();
public void Cell_Method_GetCharacters()
{
    var workbook = new Workbook();
    var worksheet = workbook.Worksheets[0];
    var commentIndex = worksheet.Comments.Add("F5");
    var comment = worksheet.Comments[commentIndex];
    Shape shape = worksheet.Shapes.AddRectangle(10, 0, 10, 0, 100, 100);
    shape.HtmlText = "aaa<div style=\"color: red;\"><i>Test1\nwwww</i></span>";
    worksheet.Cells["b3"].HtmlString = "aaa<span style=\"color: #ff0000; \">Test2\nwwww</span>";

    worksheet.Cells["A1"].HtmlString = "aaa<div style=\"color: red;\">Test3\nwwwww</div>";
    comment.HtmlNote = "Hello <div style=\"color: red;\">World\nwwww</div>";
    FontSetting[] fonts= shape.GetRichFormattings();
    CompareColor.compare("", Color.Red, fonts[2].Font.Color);
    fonts = worksheet.Cells["A1"].GetCharacters();
    CompareColor.compare("", Color.Red, fonts[1].Font.Color);
    fonts=comment.GetRichFormattings();
    CompareColor.compare("", Color.Red, fonts[1].Font.Color);

}
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| flag | Boolean | Indicates whether applying table style to the cell if the cell is in the table. |

### Return Value

All Characters objects

### Examples

```csharp
// Called: FontSetting[] fs = cell.GetCharacters(true);
public void Cell_Method_GetCharacters()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell cell = workbook.Worksheets[0].Cells["C8"];
    FontSetting[] fs = cell.GetCharacters(true);
    for (int i = 0; i < fs.Length; i++)
    {
       AssertHelper.AreEqual(Color.White, fs[i].Font.Color);
    }
}
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


