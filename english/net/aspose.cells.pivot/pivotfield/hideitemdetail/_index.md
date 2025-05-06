---
title: PivotField.HideItemDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specific PivotItem in a pivot field is hidden detail
type: docs
url: /net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Sets whether the specific PivotItem in a pivot field is hidden detail.

```csharp
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHiddenDetail | Boolean | whether the specific PivotItem is hidden |

### Examples

```csharp
// Called: firstField.HideItemDetail(2, false);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47037_&quot;;

            Workbook wb = new Workbook(filePath + &quot;SampleData.xlsx&quot;);

            PivotTable pivot = wb.Worksheets[1].PivotTables[0];
            pivot.AddFieldToArea(PivotFieldType.Page, &quot;Region&quot;);
            PivotField pageField = pivot.PageFields[0];
            pageField.CurrentPageItem = 0;

            PivotFieldCollection columnFields = pivot.ColumnFields;
            PivotField firstField = columnFields[0];
            firstField.HideItemDetail(2, false);

            pivot.RefreshData();
            pivot.CalculateData();

            Cells cells = wb.Worksheets[1].Cells;
            Assert.AreEqual(cells[&quot;H7&quot;].StringValue, &quot;3&quot;);
            Assert.AreEqual(cells[&quot;H8&quot;].StringValue, &quot;4&quot;);
            Assert.AreEqual(cells[&quot;H9&quot;].StringValue, &quot;3&quot;);
            Assert.AreEqual(cells[&quot;H10&quot;].StringValue, &quot;2&quot;);
            Assert.AreEqual(cells[&quot;H11&quot;].StringValue, &quot;1&quot;);
            Assert.AreEqual(cells[&quot;H12&quot;].StringValue, &quot;1&quot;);
            Assert.AreEqual(cells[&quot;H13&quot;].StringValue, &quot;14&quot;);
            wb.Save(CreateFolder(filePath) + &quot;out.xls&quot;);
            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


