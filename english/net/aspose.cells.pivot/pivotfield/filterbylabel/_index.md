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
// Called: field.FilterByLabel(PivotFilterType.CaptionNotContains, &amp;quot;(blank)&amp;quot;, &amp;quot;&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook book = new Workbook();
            PivotTable pivot = CreateWithBlank(book);
            PivotField field = pivot.ColumnFields[0];
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, &quot;&quot;, &quot;&quot;);

            pivot.RefreshData();
            pivot.CalculateData();
            pivot.RefreshDataOnOpeningFile = false;
            Assert.AreEqual(&quot;(blank)&quot;, book.Worksheets[0].Cells[&quot;D13&quot;].StringValue);

            field.FilterByLabel(PivotFilterType.CaptionNotEqual, &quot;(blank)&quot;, &quot;&quot;);
            pivot.CalculateData();
            Assert.AreEqual(&quot;Grand Total&quot;, book.Worksheets[0].Cells[&quot;D13&quot;].StringValue);

            field.FilterByLabel(PivotFilterType.CaptionNotContains, &quot;(blank)&quot;, &quot;&quot;);
            pivot.CalculateData();
            Assert.AreEqual(&quot;Grand Total&quot;, book.Worksheets[0].Cells[&quot;D13&quot;].StringValue);
        }
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


