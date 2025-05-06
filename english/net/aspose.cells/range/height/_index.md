---
title: Range.Height
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the width of a range in points
type: docs
url: /net/aspose.cells/range/height/
---
## Range.Height property

Gets the width of a range in points.

```csharp
public double Height { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(12.75 * 3, range.Height);
[Test]
        public void Property_Height()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange(&quot;B2:C4&quot;);
            Assert.AreEqual(12.75, range.Top);
            Assert.AreEqual(12.75 * 3, range.Height);
            Assert.AreEqual(64 /96.0 *72 , range.Left);
            Assert.AreEqual(64 / 96.0 * 72 * 2, range.Width);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


