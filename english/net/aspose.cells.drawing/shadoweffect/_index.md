---
title: Class ShadowEffect
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShadowEffect class. This class specifies the shadow effect of the chart element or shape
type: docs
url: /net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

This class specifies the shadow effect of the chart element or shape.

```csharp
public class ShadowEffect
```

## Properties

| Name | Description |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Gets and sets the blur of the shadow. Range from 0 to 100 points. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Gets and sets the color of the shadow. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Gets and sets the distance of the shadow. Range from 0 to 200 points. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Gets and sets the preset shadow type of the shadow. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |

### Examples

```csharp
// Called: ShadowEffect shadow = shape.ShadowEffect;
[Test]
        public void Type_ShadowEffect()
        {

            Workbook book = new Workbook(Constants.sourcePath + &quot;CELLSANDROID66.xlsx&quot;);

            //Access first worksheet from the collection 
            Worksheet sheet = book.Worksheets[0];

            //Access first shape from the collection 
            Shape shape = sheet.Shapes[0];

            //Get the instance of ShadowEffect from the Shape object 
            ShadowEffect shadow = shape.ShadowEffect;

            //Set its Angle, Blur, Size, Transparency and Distance properties 
            shadow.Angle = (150);
            shadow.Blur = (30);
            shadow.Size = (1.3);
            shadow.Transparency = (0.4);
            shadow.Distance = (80);
            book.Save(Constants.destPath + &quot;CELLSANDROID66.xlsx&quot;);
            book = new Workbook(Constants.destPath + &quot;CELLSANDROID66.xlsx&quot;);
            shape = book.Worksheets[0].Shapes[0];

            shadow = shape.ShadowEffect;
            Assert.AreEqual(150, shadow.Angle);
            Assert.AreEqual(30, shadow.Blur);
            Assert.AreEqual(1.3, shadow.Size);
            Assert.AreEqual(0.4, shadow.Transparency);
            Assert.AreEqual(80, shadow.Distance);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


