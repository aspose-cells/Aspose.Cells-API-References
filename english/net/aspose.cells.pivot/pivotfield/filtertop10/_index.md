---
title: PivotField.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Filters by values of data pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filters by values of data pivot field.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | Int32 | The index of data field in the data region. |
| type | PivotFilterType | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | Boolean | Indicates whether filter from top or bottom |
| itemCount | Int32 | The item count |

### Examples

```csharp
// Called: field.FilterTop10(0, PivotFilterType.Count, false, 3);
[Test]
        public void Method_Int32_()
        {
            Workbook book = AddNewWorkbok();
            PivotTable pivot = AddNewPivotTable(book);
            //Add PivotFilter
            PivotField field = pivot.RowFields[0];
            field.Method_Int32_(0, PivotFilterType.Count, false, 3);

            pivot.RefreshData();
            pivot.CalculateData();
            Assert.AreEqual(&quot;kiwi&quot;, book.Worksheets[0].Cells[&quot;A16&quot;].StringValue);
            book.Save(Constants.destPath + &quot;FilterTop10.xlsx&quot;);
            book.Save(Constants.destPath + &quot;FilterTop10.pdf&quot;);
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


