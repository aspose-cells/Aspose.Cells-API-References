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
// Called: field.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
public void PivotField_Method_FilterByDate()
{

    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    //Add PivotFilter
    PivotField field = pivot.ColumnFields[0];
    field.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));

    pivot.RefreshData();
    pivot.CalculateData();
    Assert.AreEqual("9/16/2021", book.Worksheets[0].Cells["B17"].StringValue);
    book.Save(Constants.destPath + "September.xlsx");
    book.Save(Constants.destPath + "September.pdf");
}
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


