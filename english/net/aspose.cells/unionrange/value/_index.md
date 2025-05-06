---
title: UnionRange.Value
second_title: Aspose.Cells for .NET API Reference
description: UnionRange property. Gets and sets the values of the range
type: docs
url: /net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Gets and sets the values of the range.

```csharp
public object Value { get; set; }
```

### Examples

```csharp
// Called: r.Value = &amp;quot;ABCD&amp;quot;;
[Test]
        public void Property_Value()
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


