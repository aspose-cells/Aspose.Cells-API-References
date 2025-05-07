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
// Called: field.FilterByDate(PivotFilterType.NextYear, new DateTime(now.Year - 1, now.Month, now.Day), new DateTime(now.Year + 1, 12, 31));
[Test]
        public void Method_DateTime_()
        {
            Workbook book = AddYearWorkbok();
            PivotTable pivot = AddYearPivotTable(book);

            DateTime now = DateTime.Now;

            //Add PivotFilter
            PivotField field = pivot.ColumnFields[0];
            field.FilterByDate(PivotFilterType.NextYear, new DateTime(now.Year - 1, now.Month, now.Day), new DateTime(now.Year + 1, 12, 31));

            pivot.RefreshData();
            pivot.CalculateData();
            Assert.AreEqual("460", book.Worksheets[0].Cells["C20"].StringValue);
            book.Save(Constants.destPath + "NextYear.xlsx");
            book.Save(Constants.destPath + "NextYear.pdf");
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


