---
title: ReflectionEffect.Type
second_title: Aspose.Cells for .NET API Reference
description: ReflectionEffect property. Gets and sets the preset reflection effect
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Gets and sets the preset reflection effect.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Type, ReflectionEffectType.HalfReflection4PtOffset);
[Test]
        public void Property_Type()
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

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


