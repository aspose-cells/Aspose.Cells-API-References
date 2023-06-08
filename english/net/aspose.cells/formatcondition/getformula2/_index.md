---
title: FormatCondition.GetFormula2
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition method. Gets the value or expression associated with this format condition
type: docs
url: /net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Gets the value or expression associated with this format condition.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
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

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Gets the value or expression of the conditional formatting of the cell.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
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

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

Gets the formula of the conditional formatting of the cell.

```csharp
public string GetFormula2(int row, int column)
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


