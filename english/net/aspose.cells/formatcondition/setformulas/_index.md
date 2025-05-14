---
title: FormatCondition.SetFormulas
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition method. Sets the value or expression associated with this format condition
type: docs
url: /net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Sets the value or expression associated with this format condition.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |

### Examples

```csharp
// Called: fc.SetFormulas("=1", "=2", false, false);
public void FormatCondition_Method_SetFormulas()
{
    Workbook workbook = new Workbook();
    ConditionalFormattingCollection cfs = workbook.Worksheets[0].ConditionalFormattings;
    int x = cfs.Add();
    FormatConditionCollection fcs = cfs[x];
    fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
    int index = fcs.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = fcs[index];
    fc.Operator = OperatorType.Between;
    fc.SetFormulas("=1", "=2", false, false);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    fc = workbook.Worksheets[0].ConditionalFormattings[0][0];
    Assert.AreEqual(fc.Operator, OperatorType.Between);
    Assert.AreEqual(fc.Formula1, "=1");
}
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


