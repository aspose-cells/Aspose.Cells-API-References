---
title: FontSettingCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection property. Gets the FontSetting by the index
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Gets the [`FontSetting`](../../../aspose.cells/fontsetting/) by the index.

```csharp
public FontSetting this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: fo1 = tb.TextBody[3].Font;
[Test]
        public void Property_Int32_()
        {
            Workbook w = new Workbook();
            Worksheet s = w.Worksheets[0];

            Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
            tb.Text = &quot;TextBox002&quot;;

            tb.Font.Size = 18;
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            Aspose.Cells.Font fo1 = tb.Characters(2, 4).Font;
            fo1.Color = Color.Red;
            w.Save(Constants.destPath + &quot;CELLSNET53279.xlsx&quot;);
            Workbook w1 = new Workbook(Constants.destPath + &quot;CELLSNET53279.xlsx&quot;);
            Shape x = w1.Worksheets[0].Shapes[0];
            fo1 = tb.TextBody[3].Font;
            Assert.IsTrue(fo1.IsSuperscript);

            Assert.IsTrue(Util.CompareColor(Color.Red, fo1.Color));

        }
```

### See Also

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


