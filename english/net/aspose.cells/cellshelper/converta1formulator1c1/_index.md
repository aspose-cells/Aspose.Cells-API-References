---
title: CellsHelper.ConvertA1FormulaToR1C1
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Converts A1 formula of the cell to the r1c1 formula
type: docs
url: /net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Converts A1 formula of the cell to the r1c1 formula.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The A1 formula. |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |

### Return Value

The R1C1 formula.

### Remarks

NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: string sr = CellsHelper.ConvertA1FormulaToR1C1(&amp;quot;=1+List1&amp;quot;, 1, 1);
[Test]
        public void Method_Int32_()
        {
            string sr = CellsHelper.ConvertA1FormulaToR1C1(&quot;=1+List1&quot;, 1, 1); 
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


