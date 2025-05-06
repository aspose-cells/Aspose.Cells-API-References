---
title: PivotField.FilterByDate
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Filters by date setting of row or column pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filters by date setting of row or column pivot field.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | The type of filtering data. |
| dateTime1 | DateTime | The date label of filter condition |
| dateTime2 | DateTime | The upper-bound date label of between filter condition |

### Examples

```csharp
// Called: field.FilterByDate(PivotFilterType.DateEqual, new DateTime(2021, 5, 8), new DateTime(2021, 5, 8));
[Test]
        public void Method_DateTime_()
        {
            Workbook book = AddDateWorkbok();
            PivotTable pivot = AddDatePivotTable(book);

            //Add PivotFilter
            PivotField field = pivot.ColumnFields[0];
            field.FilterByDate(PivotFilterType.DateEqual, new DateTime(2021, 5, 8), new DateTime(2021, 5, 8));

            pivot.RefreshData();
            pivot.CalculateData();
            book.Save(Constants.destPath + &quot;DateEqual.xlsx&quot;);
            book.Save(Constants.destPath + &quot;DateEqual.pdf&quot;);
            Assert.AreEqual(&quot;5/8/2021&quot;, book.Worksheets[0].Cells[&quot;B17&quot;].StringValue);
           
           
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


