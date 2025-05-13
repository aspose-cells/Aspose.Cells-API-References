---
title: FormatCondition.GetFormula1
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition method. Gets the value or expression associated with this format condition
type: docs
url: /net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Gets the value or expression associated with this format condition.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

The value or expression associated with this format condition.

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Gets the value or expression of the conditional formatting of the cell.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

The value or expression associated with the conditional formatting of the cell.

### Remarks

The given cell must be contained by this conditional formatting, otherwise null will be returned.

### Examples

```csharp
// Called: cells2[1, 0].GetFormatConditions()[0][0].GetFormula1(false, false, 1, 0),
public void FormatCondition_Method_GetFormula1()
{
    Workbook wb1 = new Workbook();
    Worksheet ss = wb1.Worksheets.Add("Source");
    FormatConditionCollection fcc = ss.ConditionalFormattings[ss.ConditionalFormattings.Add()];
    fcc.AddArea(CellArea.CreateCellArea(2, 0, 3, 0));
    fcc.AddCondition(FormatConditionType.Expression, OperatorType.None,
        "=IF(MOD(A3,2)=0,TRUE,FALSE)", null);
    Workbook wb2 = new Workbook();
    Aspose.Cells.Range range = ss.Cells.CreateRange(2, 0, 2, 1);
    Cells cells1 = wb1.Worksheets["Sheet1"].Cells;
    Cells cells2 = wb2.Worksheets["Sheet1"].Cells;
    cells1.CreateRange(0, 0, 1, 1).Copy(range);
    cells2.CreateRange(0, 0, 1, 1).Copy(range);
    Assert.AreEqual("=IF(MOD(A1,2)=0,TRUE,FALSE)",
        cells1[0, 0].GetFormatConditions()[0][0].GetFormula1(false, false, 0, 0),
        "Copy range to same workbook-A1");
    Assert.AreEqual("=IF(MOD(A2,2)=0,TRUE,FALSE)",
        cells1[1, 0].GetFormatConditions()[0][0].GetFormula1(false, false, 1, 0),
        "Copy range to same workbook-A2");
    Assert.AreEqual("=IF(MOD(A1,2)=0,TRUE,FALSE)",
        cells2[0, 0].GetFormatConditions()[0][0].GetFormula1(false, false, 0, 0),
        "Copy range to another workbook-A1");
    Assert.AreEqual("=IF(MOD(A2,2)=0,TRUE,FALSE)",
        cells2[1, 0].GetFormatConditions()[0][0].GetFormula1(false, false, 1, 0),
        "Copy range to another workbook-A2");
}
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Gets the formula of the conditional formatting of the cell.

```csharp
public string GetFormula1(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

The formula.

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


