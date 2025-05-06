---
title: MsoLineFormat.Weight
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Returns or sets the weight of the line in units of pt
type: docs
url: /net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Returns or sets the weight of the line ,in units of pt.

```csharp
public double Weight { get; set; }
```

### Examples

```csharp
// Called: t.LineFormat.Weight = 2;
[Test]
        public void Property_Weight()
        {
            Workbook book = new Workbook(); 
            Worksheet sheet = book.Worksheets[0]; 
            Aspose.Cells.Drawing.TextBox t = sheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            t.LineFormat.ForeColor = Color.Red; 
            t.LineFormat.Style = MsoLineStyle.Single;
            t.LineFormat.IsVisible = true;
            t.LineFormat.Weight = 2;
            book.Save(Constants.destPath + &quot;CellsNet23524.xlsx&quot;, SaveFormat.Xlsx);
            book = new Workbook(Constants.destPath + &quot;CellsNet23524.xlsx&quot;);
            Assert.AreEqual(book.Worksheets[0].Shapes[0].LineFormat.ForeColor.ToArgb() &amp; 0xFFFFFF, Color.Red.ToArgb() &amp; 0xffffff);


        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


