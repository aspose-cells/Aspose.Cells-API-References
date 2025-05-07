---
title: ShadowEffect.Angle
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the lighting angle. Range from 0 to 359.9 degrees
type: docs
url: /net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Gets and sets the lighting angle. Range from 0 to 359.9 degrees.

```csharp
public double Angle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual( 45,shape.ShadowEffect.Angle);
[Test]
        public void Property_Angle()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava45905.xls");
            Shape shape = workbook.Worksheets[0].Shapes[3];
            Assert.AreEqual( 45,shape.ShadowEffect.Angle);
            Assert.AreEqual(8, workbook.Worksheets[0].Shapes[2].Font.Size);
            workbook.Save(Constants.destPath + "CellsJava45905.xls");
        }
```

### See Also

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


