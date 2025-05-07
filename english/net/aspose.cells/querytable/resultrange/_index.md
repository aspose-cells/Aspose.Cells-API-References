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
// Called: Assert.AreEqual("A1:A8", qt.ResultRange.Address);
[Test]
        public void Property_ResultRange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells46297.xlsx");
            QueryTable qt = workbook.Worksheets[0].QueryTables[0];
           Assert.AreEqual("A1:A8", qt.ResultRange.Address);
        }
```

### See Also

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


