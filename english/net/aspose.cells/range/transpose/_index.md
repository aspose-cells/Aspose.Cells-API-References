---
title: Range.Transpose
second_title: Aspose.Cells for .NET API Reference
description: Range method. Transpose rotate data from rows to columns or vice versa
type: docs
url: /net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transpose (rotate) data from rows to columns or vice versa.

```csharp
public void Transpose()
```

### Examples

```csharp
// Called: c.Transpose();
[Test]
        public void Method_Transpose()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + (&quot;CellsNet55526.xlsx&quot;));
            Aspose.Cells.Range c = workbook.Worksheets[&quot;Sheet4&quot;].Cells.CreateRange(&quot;A1:C3&quot;);
            c.Transpose();
            Assert.AreEqual(&quot;6&quot;, workbook.Worksheets[3].Cells[&quot;B3&quot;].StringValue);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


