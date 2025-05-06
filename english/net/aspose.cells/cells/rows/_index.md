---
title: Cells.Rows
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Row objects that represents the individual rows in this worksheet
type: docs
url: /net/aspose.cells/cells/rows/
---
## Cells.Rows property

Gets the collection of [`Row`](../../row/) objects that represents the individual rows in this worksheet.

```csharp
public RowCollection Rows { get; }
```

### Examples

```csharp
// Called: var r3 = workbook.Worksheets[0].Cells.Rows.Count; // =5
[Test]
        public void Property_Rows()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;sl1r.xls&quot;);
            var r1 = workbook.Worksheets[0].Cells.Rows.Count; // =5
            var r2 = workbook.Worksheets[0].Cells.MaxDataRow; // =4
            workbook.Worksheets[0].Cells.DeleteBlankRows();
            var r3 = workbook.Worksheets[0].Cells.Rows.Count; // =5
            var r4 = workbook.Worksheets[0].Cells.MaxDataRow; // =4
            Assert.AreEqual(r3, 2);
            Assert.AreEqual(r4, 1);
        }
```

### See Also

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


