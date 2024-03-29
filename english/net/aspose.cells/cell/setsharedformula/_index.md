---
title: Cell.SetSharedFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets a formula to a range of cells
type: docs
url: /net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Sets a formula to a range of cells.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| isR1C1 | Boolean | whether the formula is R1C1 formula |
| isLocal | Boolean | whether the formula is locale formatted |

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Sets shared formulas to a range of cells.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Sets shared formulas to a range of cells.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Sets shared formulas to a range of cells.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given shared formula |

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


