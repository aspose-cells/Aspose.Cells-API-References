---
title: Cells.ConvertStringToNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Converts all string data in the worksheet to numeric value if possible
type: docs
url: /net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Converts all string data in the worksheet to numeric value if possible.

```csharp
public void ConvertStringToNumericValue()
```

### Examples

```csharp
// Called: cells.ConvertStringToNumericValue();
[Test]
        public void Method_ConvertStringToNumericValue()
        {
            Workbook workbook = new Workbook();
           
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;(123)&quot;);
            cells[&quot;A2&quot;].PutValue(&quot;123&quot;);
            cells.ConvertStringToNumericValue();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].DoubleValue, -123);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A2&quot;].DoubleValue, 123);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


