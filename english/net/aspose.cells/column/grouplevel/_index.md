---
title: Column.GroupLevel
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets the group level of the column
type: docs
url: /net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Gets the group level of the column.

```csharp
public byte GroupLevel { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells.Columns[0].GroupLevel, 0);
[Test]
        public void Property_GroupLevel()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;sdfsdfsdf&quot;);
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(Constants.destPath + &quot;GroupLevel0.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;GroupLevel0.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells.Columns[0].GroupLevel, 0);
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


