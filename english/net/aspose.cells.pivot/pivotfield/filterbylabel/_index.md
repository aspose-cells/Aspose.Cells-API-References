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
// Called: field.FilterByLabel(PivotFilterType.CaptionNotContains, "(blank)", "");
public void PivotField_Method_FilterByLabel()
{
    Workbook book = new Workbook();
    PivotTable pivot = CreateWithBlank(book);
    PivotField field = pivot.ColumnFields[0];
    field.FilterByLabel(PivotFilterType.CaptionNotEqual, "", "");

    pivot.RefreshData();
    pivot.CalculateData();
    pivot.RefreshDataOnOpeningFile = false;
    Assert.AreEqual("(blank)", book.Worksheets[0].Cells["D13"].StringValue);

    field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
    pivot.CalculateData();
    Assert.AreEqual("Grand Total", book.Worksheets[0].Cells["D13"].StringValue);

    field.FilterByLabel(PivotFilterType.CaptionNotContains, "(blank)", "");
    pivot.CalculateData();
    Assert.AreEqual("Grand Total", book.Worksheets[0].Cells["D13"].StringValue);
}
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


