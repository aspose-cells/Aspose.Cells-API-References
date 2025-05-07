---
title: ReflectionEffect.Transparency
second_title: Aspose.Cells for .NET API Reference
description: ReflectionEffect property. Gets and sets the degree of the starting reflection transparency as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Transparency, 0.5);
[Test]
        public void Property_Transparency()
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


