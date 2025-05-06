---
title: ListObject.ShowTotals
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this ListObject show total row
type: docs
url: /net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Gets and sets whether this ListObject show total row.

```csharp
public bool ShowTotals { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].ListObjects[0].ShowTotals);
[Test]
        public void Property_ShowTotals()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;N45670.xls&quot;);
            Assert.IsFalse(workbook.Worksheets[0].ListObjects[0].ShowTotals);
            workbook.Save(Constants.destPath + &quot;N45670.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;N45670.xls&quot;);
            Assert.IsFalse(workbook.Worksheets[0].ListObjects[0].ShowTotals);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


