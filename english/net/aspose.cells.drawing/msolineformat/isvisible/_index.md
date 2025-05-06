---
title: MsoLineFormat.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Indicates whether the object is visible
type: docs
url: /net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Indicates whether the object is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(shape.LineFormat.IsVisible);
[Test]
        public void Property_IsVisible()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int columnNumber = 0;

            int rowNumber = 0;

            int textboxIndex = worksheet.TextBoxes.Add(rowNumber, columnNumber, 100, 100);

            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];

            textbox.Text = &quot;sdfafasdfasdf&quot;;

            textbox.Placement = PlacementType.FreeFloating;

            textbox.Font.Color = Color.Black;

            textbox.Font.Size = 10;

            MsoFillFormat fillformat = textbox.FillFormat;

            // fillformat.ForeColor = System.Drawing.Color.White;
            fillformat.IsVisible = false;

            MsoLineFormat lineformat = textbox.LineFormat;

            lineformat.IsVisible = false;
            workbook.Save(Constants.destPath + &quot;CellsNet44494.ods&quot;);
            // workbook.Save(path + &quot;dest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet44494.ods&quot;);
            Shape shape = workbook.Worksheets[0].Shapes[0];
            Assert.IsFalse(shape.FillFormat.IsVisible);
            Assert.IsFalse(shape.LineFormat.IsVisible);
        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


