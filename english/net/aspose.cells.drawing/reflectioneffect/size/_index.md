---
title: ReflectionEffect.Size
second_title: Aspose.Cells for .NET API Reference
description: ReflectionEffect property. Gets and sets the end position along the alpha gradient ramp of the end alpha valuein unit of percentage
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage

```csharp
public double Size { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Size, 55.5);
public void ReflectionEffect_Property_Size()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestRelection1.xlsx");
    Shape shape = workbook.Worksheets[0].Shapes[0];
    ReflectionEffect r = shape.Reflection;
    Assert.AreEqual(r.Type, ReflectionEffectType.HalfReflection4PtOffset);
    Assert.AreEqual(r.Transparency, 0.5);
    Assert.AreEqual(r.Size, 55.5);
    Assert.AreEqual(r.Blur, 0.5);
    Assert.AreEqual(r.Distance, 4);
    workbook.Save(Constants.destPath + "TestRelection1.xlsx");
    workbook = new Workbook(Constants.destPath + "TestRelection1.xlsx");
    shape = workbook.Worksheets[0].Shapes[0];
    r = shape.Reflection;
    Assert.AreEqual(r.Type, ReflectionEffectType.HalfReflection4PtOffset);
    Assert.AreEqual(r.Transparency, 0.5);
    Assert.AreEqual(r.Size, 55.5);
    Assert.AreEqual(r.Blur, 0.5);
    Assert.AreEqual(r.Distance, 4);

           
}
```

### See Also

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


