---
title: PivotField.ShowValuesAs
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Shows values of data field as different display format when the ShowDataAs calculation is in use
type: docs
url: /net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## PivotField.ShowValuesAs method

Shows values of data field as different display format when the ShowDataAs calculation is in use.

```csharp
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | The data display format type. |
| baseField | Int32 | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | PivotItemPositionType | The position type of base iteam. |
| baseItem | Int32 | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### Remarks

Only for data field.

### Examples

```csharp
// Called: pt.DataFields[0].ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Custom, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET55698.xlsx");
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
              pt.DataFields[0].ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Custom, 0);
            Assert.IsTrue(pt.AutofitColumnWidthOnUpdate);
            Assert.AreEqual(PivotMissingItemLimitType.Automatic, pt.MissingItemsLimit);
            Assert.AreEqual(PivotFieldDataDisplayFormat.DifferenceFrom, pt.DataFields[0].ShowValuesSetting.CalculationType);

        }
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


