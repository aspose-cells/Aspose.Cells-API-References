---
title: Bevel.Width
second_title: Aspose.Cells for .NET API Reference
description: Bevel property. Gets and sets the width of the bevel or how far into the shape it is applied. In unit of Points
type: docs
url: /net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points.

```csharp
public double Width { get; set; }
```

### Examples

```csharp
// Called: bevel.Width = 6;
[Test]
        //http://www.aspose.com/community/forums/thread/221034.aspx
        public void Property_Width()
        {
            Console.WriteLine(&quot;Property_Width()&quot;);
            string infn = path + &quot;Test_BevelEffectOnBubble.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_BevelEffectOnBubble_out.xlsx&quot;;

            Workbook book = new Workbook(infn);
            Chart c = book.Worksheets[0].Charts[0];
            Series ser = c.NSeries[0];
            ShapePropertyCollection spPr = ser.ShapeProperties;
            Bevel bevel = spPr.Format3D.TopBevel;
            bevel.Type = BevelPresetType.Circle;
            bevel.Height = 6;
            bevel.Width = 6;

            book.Save(outfn);
        }
```

### See Also

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


