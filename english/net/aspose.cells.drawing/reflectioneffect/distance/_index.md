---
title: ReflectionEffect.Distance
second_title: Aspose.Cells for .NET API Reference
description: ReflectionEffect property. Gets and sets how far to distance the shadowin unit of points
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Gets and sets how far to distance the shadow,in unit of points.

```csharp
public double Distance { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Distance, 0);
[Test]
        public void Property_Distance()
        {
            var book = new Workbook();
            book.Worksheets[0].Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            ReflectionEffect relection = book.Worksheets[0].Shapes[0].Reflection;
            Assert.AreEqual(ReflectionEffectType.None, relection.Type);

            Console.WriteLine(relection.Type);
            relection.Type = ReflectionEffectType.HalfReflectionTouching;

            book.Save(Constants.destPath + "TestRelection2.xlsx");
            book = new Workbook(Constants.destPath + "TestRelection2.xlsx");
            ReflectionEffect r = book.Worksheets[0].Shapes[0].Reflection;
            Assert.AreEqual(ReflectionEffectType.HalfReflectionTouching, relection.Type);
            Assert.AreEqual(r.Transparency, 0.5);
            Assert.AreEqual(r.Size, 55);
            Assert.AreEqual(r.Blur, 0.5);
            Assert.AreEqual(r.Distance, 0);
        }
```

### See Also

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


