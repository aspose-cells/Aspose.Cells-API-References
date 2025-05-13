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
public void PivotField_Method_HideItemDetail()
{
    string filePath = Constants.PivotTableSourcePath + @"NET47037_";

    Workbook wb = new Workbook(filePath + "SampleData.xlsx");

    PivotTable pivot = wb.Worksheets[1].PivotTables[0];
    pivot.AddFieldToArea(PivotFieldType.Page, "Region");
    PivotField pageField = pivot.PageFields[0];
    pageField.CurrentPageItem = 0;

    PivotFieldCollection columnFields = pivot.ColumnFields;
    PivotField firstField = columnFields[0];
    firstField.HideItemDetail(2, false);

    pivot.RefreshData();
    pivot.CalculateData();

    Cells cells = wb.Worksheets[1].Cells;
    Assert.AreEqual(cells["H7"].StringValue, "3");
    Assert.AreEqual(cells["H8"].StringValue, "4");
    Assert.AreEqual(cells["H9"].StringValue, "3");
    Assert.AreEqual(cells["H10"].StringValue, "2");
    Assert.AreEqual(cells["H11"].StringValue, "1");
    Assert.AreEqual(cells["H12"].StringValue, "1");
    Assert.AreEqual(cells["H13"].StringValue, "14");
    wb.Save(CreateFolder(filePath) + "out.xls");
    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


