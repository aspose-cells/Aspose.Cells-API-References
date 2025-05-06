---
title: ThreeDFormat.TopBevelHeight
second_title: Aspose.Cells for .NET API Reference
description: ThreeDFormat property. Gets and sets the height of the top bevel or how far into the shape it is applied. In unit of Points
type: docs
url: /net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points.

```csharp
public double TopBevelHeight { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual( n3df.TopBevelHeight , 30);//this is not taking effect
[Test]
        public void Property_TopBevelHeight()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET44830.xlsx&quot;);
            //Access first worksheet 
            Worksheet ws = wb.Worksheets[0];

            //Access first shape 
            Shape sh = ws.Shapes[0];

            //Apply different three dimensional settings 
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = BevelType.HardEdge;
            n3df.TopBevelWidth = 30; //this is not taking effect 
            n3df.TopBevelHeight = 30;//this is not taking effect 

            //Save the output excel file in xlsx format 
            wb.Save(Constants.destPath + &quot;CELLSNET44830.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET44830.xlsx&quot;);
            sh = ws.Shapes[0];

            //Apply different three dimensional settings 
            n3df = sh.ThreeDFormat;
           Assert.AreEqual(n3df.ContourWidth,17);
            Assert.AreEqual(n3df.ExtrusionHeight,32);
            Assert.AreEqual(n3df.TopBevelType , BevelType.HardEdge);
            Assert.AreEqual(n3df.TopBevelWidth , 30); //this is not taking effect 
           Assert.AreEqual( n3df.TopBevelHeight , 30);//this is not taking effect 

        }
```

### See Also

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


