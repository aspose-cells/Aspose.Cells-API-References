---
title: UnionRange.HasRange
second_title: Aspose.Cells for .NET API Reference
description: UnionRange property. Indicates whether this has range
type: docs
url: /net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Indicates whether this has range.

```csharp
public bool HasRange { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(r.HasRange);
[Test]
        public void Property_HasRange()
        {
            Workbook workbook = new Workbook();
            UnionRange r = workbook.Worksheets.CreateUnionRange(&quot;A1:A10,C1:C10&quot;, 0);
            Assert.IsTrue(r.HasRange);
            r.Value = &quot;ABCD&quot;;
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Red;
            workbook.Save(Constants.destPath + &quot;CellsNet47054.xlsx&quot;);

        }
```

### See Also

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


