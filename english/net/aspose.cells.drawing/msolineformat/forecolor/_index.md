---
title: MsoLineFormat.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Gets and sets the border line fore color
type: docs
url: /net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Gets and sets the border line fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(book.Worksheets[0].Shapes[0].LineFormat.ForeColor.ToArgb() & 0xFFFFFF, Color.Red.ToArgb() & 0xffffff);
[Test]
        public void Property_ForeColor()
        {
            Workbook book = new Workbook(); 
            Worksheet sheet = book.Worksheets[0]; 
            Aspose.Cells.Drawing.TextBox t = sheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            t.LineFormat.ForeColor = Color.Red; 
            t.LineFormat.Style = MsoLineStyle.Single;
            t.LineFormat.IsVisible = true;
            t.LineFormat.Weight = 2;
            book.Save(Constants.destPath + "CellsNet23524.xlsx", SaveFormat.Xlsx);
            book = new Workbook(Constants.destPath + "CellsNet23524.xlsx");
            Assert.AreEqual(book.Worksheets[0].Shapes[0].LineFormat.ForeColor.ToArgb() & 0xFFFFFF, Color.Red.ToArgb() & 0xffffff);


        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


