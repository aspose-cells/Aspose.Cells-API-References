---
title: FontSettingCollection.Replace
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection method. Replace the text
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Replace the text.

```csharp
public void Replace(int index, int count, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The start index. |
| count | Int32 | The count of characters. |
| text | String | The text. |

### See Also

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Replace the text.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | String | The old text. |
| newValue | String | The new text. |

### Examples

```csharp
// Called: shape.TextBody.Replace("３４", "ABC");
public void FontSettingCollection_Method_Replace()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    Shape shape = worksheet.Shapes[0];
          
    shape.TextBody.Replace("３４", "ABC");
    int index = shape.Text.IndexOf("ABC");
   Assert.AreEqual(FontUnderlineType.Single, shape.Characters(index, 2).Font.Underline);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


