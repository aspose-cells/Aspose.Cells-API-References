---
title: ThreeDFormat.ExtrusionHeight
second_title: Aspose.Cells for .NET API Reference
description: ThreeDFormat property. Gets and sets the extrusion height of the applied to the shape in unit of points
type: docs
url: /net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

Gets and sets the extrusion height of the applied to the shape, in unit of points.

```csharp
public double ExtrusionHeight { get; set; }
```

### Examples

```csharp
// Called: n3df.ExtrusionHeight = 32;
[Test]
        public void Property_ExtrusionHeight()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET44830.xlsx");
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
            wb.Save(Constants.destPath + "CELLSNET44830.xlsx");
            wb = new Workbook(Constants.destPath + "CELLSNET44830.xlsx");
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


