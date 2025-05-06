---
title: Range.Value
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets and sets the value of the range
type: docs
url: /net/aspose.cells/range/value/
---
## Range.Value property

Gets and sets the value of the range.

```csharp
public object Value { get; set; }
```

### Remarks

If the range contains multiple cells, the returned/applied object should be a two-dimension Array object.

### Examples

```csharp
// Called: r.Value = new int[3, 3];
[Test]
        public void Property_Value()
        {
            Workbook workbook = new Workbook();

            Aspose.Cells.Range r = workbook.Worksheets[0].Cells.CreateRange(&quot;A1&quot;);
            r.Value = new int[3, 3];
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;B2&quot;].IntValue, 0);
            workbook.Save(Constants.destPath + &quot;CELLSNET51184.xlsx&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


