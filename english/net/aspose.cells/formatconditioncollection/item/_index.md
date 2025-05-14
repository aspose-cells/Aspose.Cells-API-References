---
title: FormatConditionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets the formatting condition by index
type: docs
url: /net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Gets the formatting condition by index.

```csharp
public FormatCondition this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | the index of the formatting condition to return. |

### Return Value

the formatting condition

### Examples

```csharp
// Called: Assert.AreEqual("=ABS(#REF!)", fcc[0].Formula2, "Copied formula2 of format condition");
public void FormatConditionCollection_Property_Item()
{
    Workbook wbDest = new Workbook(FileFormatType.Excel97To2003);
    Workbook wbSrc = new Workbook(FileFormatType.Xlsx);
    Worksheet sheet = wbSrc.Worksheets[0];
    sheet.Name = "Copied";
    sheet.ConditionalFormattings.Add();
    FormatConditionCollection fcc = sheet.ConditionalFormattings[0];
    fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
        FormatConditionType.CellValue, OperatorType.Between, "=ABS($A$1048000)", "=ABS($B$1048000)");
    Validation vldt = sheet.Validations[sheet.Validations.Add(CellArea.CreateCellArea(0, 0, 0, 3))];
    vldt.Operator = OperatorType.Between;
    vldt.Formula1 = "=ABS($A$1048000)";
    vldt.Formula2 = "=ABS($B$1048000)";
    wbDest.Combine(wbSrc);
    sheet = wbDest.Worksheets["Copied"];
    fcc = sheet.ConditionalFormattings[0];
    Assert.AreEqual("=ABS(#REF!)", fcc[0].Formula1, "Copied formula1 of format condition");
    Assert.AreEqual("=ABS(#REF!)", fcc[0].Formula2, "Copied formula2 of format condition");
    vldt = sheet.Validations[0];
    Assert.AreEqual("=ABS(#REF!)", vldt.Formula1, "Copied formula1 of validation");
    Assert.AreEqual("=ABS(#REF!)", vldt.Formula2, "Copied formula2 of validation");
}
```

### See Also

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


