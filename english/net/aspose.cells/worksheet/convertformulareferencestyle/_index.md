---
title: Worksheet.ConvertFormulaReferenceStyle
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Converts the formula reference style
type: docs
url: /net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Converts the formula reference style.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula to be converted. |
| toR1C1 | Boolean | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |

### Return Value

The converted formula.

### Examples

```csharp
// Called: Assert.AreEqual("$W1,testDS,rcurr,$X1", sheet.ConvertFormulaReferenceStyle(fml, false, 0, 0), fml);
public void Worksheet_Method_ConvertFormulaReferenceStyle()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    string fml = "R[0]C23,testDS,R[0]C24";
    Assert.AreEqual("$W1,testDS,$X1", sheet.ConvertFormulaReferenceStyle(fml, false, 0, 0), fml);
    fml = "R[0]C23,testDS,rcurr,R[0]C24";
    Assert.AreEqual("$W1,testDS,rcurr,$X1", sheet.ConvertFormulaReferenceStyle(fml, false, 0, 0), fml);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


