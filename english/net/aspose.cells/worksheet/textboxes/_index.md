---
title: Worksheet.TextBoxes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a TextBox collection
type: docs
url: /net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Gets a [`TextBox`](../../../aspose.cells.drawing/textbox/) collection.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Examples

```csharp
// Called: TextBox t = ws.TextBoxes[tID];
public void Worksheet_Property_TextBoxes()
{

    Workbook wb = new Workbook();
    Worksheet ws = wb.Worksheets[0];

    int tID = ws.TextBoxes.Add(1, 1, 500, 1000);

    TextBox t = ws.TextBoxes[tID];

    t.Text = ("Red text 1. Plain text 1. Red text 2. Plain text 2.");
    t.Characters(26, 10).Font.Color = (Color.DarkRed);
    t.Characters(0, 10).Font.Color = (Color.Red);

    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(wb.Worksheets[0].TextBoxes[0].Text, "Red text 1. Plain text 1. Red text 2. Plain text 2.");
}
```

### See Also

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


