---
title: ReflectionEffect.Blur
second_title: Aspose.Cells for .NET API Reference
description: ReflectionEffect property. Gets and sets the blur radiusin unit of points
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Gets and sets the blur radius,in unit of points.

```csharp
public double Blur { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Blur, 0.5);
[Test]
        public void Property_Blur()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestRelection1.xlsx&quot;);
            Shape shape = workbook.Worksheets[0].Shapes[0];
            ReflectionEffect r = shape.Reflection;
            Assert.AreEqual(r.Type, ReflectionEffectType.HalfReflection4PtOffset);
            Assert.AreEqual(r.Transparency, 0.5);
            Assert.AreEqual(r.Size, 55.5);
            Assert.AreEqual(r.Blur, 0.5);
            Assert.AreEqual(r.Distance, 4);
            workbook.Save(Constants.destPath + &quot;TestRelection1.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestRelection1.xlsx&quot;);
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


