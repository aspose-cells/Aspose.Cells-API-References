---
title: CellsHelper.ConvertR1C1FormulaToA1
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Converts the r1c1 formula of the cell to A1 formula
type: docs
url: /net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Converts the r1c1 formula of the cell to A1 formula.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| r1c1Formula | String | The r1c1 formula. |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |

### Return Value

The A1 formula.

### Remarks

NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: string a11 = CellsHelper.ConvertR1C1FormulaToA1(a1, 0, 0);
[Test]
	    public void Method_Int32_()
	    {
            Workbook wk = new Workbook(Constants.sourcePath + "Formula/CellsJava42111.xlsx");
            string a1 = wk.Worksheets[0].Cells["A1"].R1C1Formula;
            string b1 = wk.Worksheets[0].Cells["B1"].R1C1Formula;
            string a2 = wk.Worksheets[0].Cells["A2"].R1C1Formula;
            string b2 = wk.Worksheets[0].Cells["B2"].R1C1Formula;
            Assert.AreEqual(a1, "=R[1048575]C");
            Assert.AreEqual(b1,"=R[1048574]C");
            Assert.AreEqual(a2, "=R1048576C");
            Assert.AreEqual(b2, "=R1048575C");
            //      wk.Worksheets[0].Cells.DeleteRows(17, 9);
            string a11 = CellsHelper.ConvertR1C1FormulaToA1(a1, 0, 0);
            string a22 = CellsHelper.ConvertR1C1FormulaToA1(a2, 0, 0);
            string b11 = CellsHelper.ConvertR1C1FormulaToA1(b1, 0, 1);
            string b22 = CellsHelper.ConvertR1C1FormulaToA1(b2, 0, 1);
            Assert.AreEqual(a11, "=A1048576");
            Assert.AreEqual(b11, "=B1048575");
            Assert.AreEqual(a22, "=A$1048576");
            Assert.AreEqual(b22, "=B$1048575");
	    }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


