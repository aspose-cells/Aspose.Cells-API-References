---
title: Series.ShapeProperties
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the ShapePropertyCollection object that holds the visual shape properties of the Series
type: docs
url: /net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Gets the [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) object that holds the visual shape properties of the Series.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Examples

```csharp
// Called: ShapePropertyCollection spPr = ser.ShapeProperties;
[Test]
        //http://www.aspose.com/community/forums/thread/221034.aspx
        public void Property_ShapeProperties()
        {
            Console.WriteLine("Property_ShapeProperties()");
            string infn = path + "Test_BevelEffectOnBubble.xlsx";
            string outfn = Constants.destPath + "Test_BevelEffectOnBubble_out.xlsx";

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

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


