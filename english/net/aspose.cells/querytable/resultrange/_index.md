---
title: QueryTable.ResultRange
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the range of the result
type: docs
url: /net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Gets the range of the result.

```csharp
public Range ResultRange { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;A1:A8&amp;quot;, qt.ResultRange.Address);
[Test]
        public void Property_ResultRange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cells46297.xlsx&quot;);
            QueryTable qt = workbook.Worksheets[0].QueryTables[0];
           Assert.AreEqual(&quot;A1:A8&quot;, qt.ResultRange.Address);
        }
```

### See Also

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


