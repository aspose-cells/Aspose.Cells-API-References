---
title: Cell.BoolValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the boolean value contained in the cell
type: docs
url: /net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Gets the boolean value contained in the cell.

```csharp
public bool BoolValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, cell.BoolValue); //=&amp;quot;3&amp;quot;&amp;gt;&amp;quot;3&amp;quot;
[Test]
        public void Property_BoolValue()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.Formula = &quot;=\&quot;3\&quot;&gt;\&quot;3\&quot;&quot;;
            Console.WriteLine(&quot;=\&quot;3\&quot;&gt;\&quot;3\&quot;&quot;);
            workbook.CalculateFormula();
            Assert.AreEqual(false, cell.BoolValue); //=&quot;3&quot;&gt;&quot;3&quot;
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


