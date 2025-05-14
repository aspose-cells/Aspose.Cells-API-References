---
title: ShadowEffect.Transparency
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the degree of transparency of the shadow. Range from 0.0 opaque to 1.0 clear
type: docs
url: /net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: shadow.Transparency = (0.4);
public void ShadowEffect_Property_Transparency()
{

    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");

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
    book.Save(Constants.destPath + "example.xlsx");
    book = new Workbook(Constants.destPath + "example.xlsx");
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

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


