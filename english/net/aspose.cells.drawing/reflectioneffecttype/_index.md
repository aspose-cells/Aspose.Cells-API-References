---
title: Enum ReflectionEffectType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ReflectionEffectType enum. Represents the effect type of reflection
type: docs
url: /net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Represents the effect type of reflection.

```csharp
public enum ReflectionEffectType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No reflection effect. |
| Custom | `1` | Custom reflection effect. |
| TightReflectionTouching | `2` | Tight reflection, touching. |
| HalfReflectionTouching | `3` | Half reflection, touching. |
| FullReflectionTouching | `4` | Full reflection, touching. |
| TightReflection4PtOffset | `5` | Tight reflection, 4 pt offset. |
| HalfReflection4PtOffset | `6` | Half reflection, 4 pt offset. |
| FullReflection4PtOffset | `7` | Full reflection, 4 pt offset. |
| TightReflection8PtOffset | `8` | Tight reflection, 8 pt offset. |
| HalfReflection8PtOffset | `9` | Half reflection, 8 pt offset. |
| FullReflection8PtOffset | `10` | Full reflection, 8 pt offset. |

### Examples

```csharp
// Called: Assert.AreEqual(ReflectionEffectType.HalfReflectionTouching, relection.Type);
[Test]
        public void Type_ReflectionEffectType()
        {
            var book = new Workbook();
            book.Worksheets[0].Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            ReflectionEffect relection = book.Worksheets[0].Shapes[0].Reflection;
            Assert.AreEqual(ReflectionEffectType.None, relection.Type);

            Console.WriteLine(relection.Type);
            relection.Type = ReflectionEffectType.HalfReflectionTouching;

            book.Save(Constants.destPath + &quot;TestRelection2.xlsx&quot;);
            book = new Workbook(Constants.destPath + &quot;TestRelection2.xlsx&quot;);
            ReflectionEffect r = book.Worksheets[0].Shapes[0].Reflection;
            Assert.AreEqual(ReflectionEffectType.HalfReflectionTouching, relection.Type);
            Assert.AreEqual(r.Transparency, 0.5);
            Assert.AreEqual(r.Size, 55);
            Assert.AreEqual(r.Blur, 0.5);
            Assert.AreEqual(r.Distance, 0);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


