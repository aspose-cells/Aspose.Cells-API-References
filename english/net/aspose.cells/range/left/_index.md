---
title: Range.Left
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the distance in points from the left edge of column A to the left edge of the range
type: docs
url: /net/aspose.cells/range/left/
---
## Range.Left property

Gets the distance, in points, from the left edge of column A to the left edge of the range.

```csharp
public double Left { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(64 /96.0 *72 , range.Left);
[Test]
        public void Property_Left()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B2:C4");
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


