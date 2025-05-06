---
title: TextEffectFormat.Text
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. The text in the WordArt
type: docs
url: /net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

The text in the WordArt.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sheet.Shapes[0].TextEffect.Text, &amp;quot;Opps!&amp;quot;);
[Test]
        public void Property_Text()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-41731.xls&quot;);
            Worksheet sheet = workbook.Worksheets[2];
            sheet.Cells[&quot;M10&quot;].PutValue(&quot;Opps!&quot;);

            workbook.CalculateFormula();
            sheet.Shapes.UpdateSelectedValue();
            Assert.AreEqual(sheet.Shapes[0].TextEffect.Text, &quot;Opps!&quot;);
           
        }
```

### See Also

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


