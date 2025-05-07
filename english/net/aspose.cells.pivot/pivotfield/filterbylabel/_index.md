---
title: PivotField.FilterByLabel
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Filters by captions of row or column pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filters by captions of row or column pivot field.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | The type of filtering data. |
| label1 | String | The label of filter condition |
| label2 | String | The upper-bound label of between filter condition |

### Examples

```csharp
// Called: field.FilterByLabel(PivotFilterType.CaptionGreaterThanOrEqual, "2020", "");
[Test]
        public void Method_String_()
        {
            Workbook book = AddNewWorkbok();
            PivotTable pivot = AddNewPivotTable(book);


            //Add PivotFilter
            PivotField field = pivot.ColumnFields[0];
            field.FilterByLabel(PivotFilterType.CaptionGreaterThanOrEqual, "2020", "");

            pivot.RefreshData();
            pivot.CalculateData();
            Assert.AreEqual("2020", book.Worksheets[0].Cells["B13"].StringValue);
            book.Save(Constants.destPath + "CaptionGreaterThanOrEqual.xlsx");
            book.Save(Constants.destPath + "CaptionGreaterThanOrEqual.pdf");
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


