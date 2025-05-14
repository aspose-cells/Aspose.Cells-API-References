---
title: Cell.SetArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets an array formula to a range of cells
type: docs
url: /net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Sets an array formula to a range of cells.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| isR1C1 | Boolean | whether the formula is R1C1 formula |
| isLocal | Boolean | whether the formula is locale formatted |

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int) {#setarrayformula}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |

### Examples

```csharp
// Called: cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);
public void Cell_Method_SetArrayFormula()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);
    Console.WriteLine("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})");
    workbook.CalculateFormula();
    Assert.AreEqual(0, cells[0, 0].IntValue);
    Assert.AreEqual(0, cells[1, 0].IntValue);
    Assert.AreEqual(0, cells[2, 0].IntValue);
    Assert.AreEqual(0, cells[3, 0].IntValue);//=FREQUENCY({"79","85","78","85","50","81","95","88","97"},{70,79,89})
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Sets an array formula to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### Examples

```csharp
// Called: cells[1, 0].SetArrayFormula("=TRANSPOSE(Sheet1!C1:E1)", 2, 1, new FormulaParseOptions());
public void Cell_Method_SetArrayFormula()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets.Add("Sheet2").Cells;
    cells[1, 0].SetArrayFormula("=TRANSPOSE(Sheet1!C1:E1)", 2, 1, new FormulaParseOptions());
    cells[1, 1].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!C1:E1)", new FormulaParseOptions(), false);

    cells = wb.Worksheets[0].Cells;
    cells[0, 0].Formula = "=B1";
    cells[0, 1].PutValue(1);
    cells[0, 2].PutValue(2);
    cells[0, 3].PutValue(4);
    cells[0, 4].PutValue(8);
    string[] fmls = new string[]
    {
        "=TRANSPOSE(C1:E1)", "=TRANSPOSE(C1:E1)",
        "=B1#", "=$A$3#", "=INDIRECT(\"A2:B2\")#",
        "=SUM(A2#)", "=$A$1#", "=SUM(Sheet2!A2#)",
        "=A2#", "=INDIRECT(\"A2:A2\")#", "=Sheet2!A2#",
        "=$B$2#", "=Sheet2!A2#:Sheet2!B2#",
    };
    int[][] vals = new int[][]
    {
        new int[]{2, 4, }, new int[]{2, 4, 8, },
        null, null, null,
        new int[]{6, }, new int[]{1, }, new int[]{6, },
        new int[]{2, 4, }, new int[]{2, 4, }, new int[]{2, 4, },
        new int[]{2, 4, 8, }, new int[]{2, 4, 0, }, new int[]{2, 4, 8, },
    };
    cells[1, 0].SetArrayFormula(fmls[0], 2, 1, new FormulaParseOptions());
    wb.CalculateFormula();
    for (int i = 1; i < fmls.Length; i++)
    {
        cells[1, i].SetDynamicArrayFormula(fmls[i], new FormulaParseOptions(), true);
    }

    for (int i = 0; i < 2; i++)
    {
        if (i > 0)
        {
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            cells = wb.Worksheets[0].Cells;
        }
        for (int j = 0; j < fmls.Length; j++)
        {
            int[] cv = vals[j];
            int h = cv == null ? 1 : cv.Length;
            for (int k = h; k > 0; k--)
            {
                Assert.AreEqual(fmls[j], cells[k, j].Formula,
                    ((char)('A' + j)) + "" + (k + 1) + ".Formula");
            }
            for (int k = h; k < 3; k++)
            {
                Assert.IsNull(cells.CheckCell(k + 1, j), fmls[j]
                    + " should not be spilled to " + ((char)('A' + j)) + "" + (k + 2));
            }
        }
        for (int k = 1; k < 4; k++)
        {
            Assert.AreEqual(fmls[fmls.Length - 1], cells[k, fmls.Length].Formula,
                ((char)('A' + fmls.Length)) + "" + (k + 1) + ".Formula");
        }
        wb.CalculateFormula(false);
        for (int j = 0; j < vals.Length; j++)
        {
            int[] cv = vals[j];
            if (cv == null)
            {
                Cell cell = cells[1, j];
                Assert.AreEqual("#REF!", cell.Value,
                    cell.Name + ".Value(Formula=" + cell.Formula + ")");
                continue;
            }
            for (int k = 0; k < cv.Length; k++)
            {
                Cell cell = cells[k + 1, j];
                Assert.AreEqual(cv[k], cell.IntValue,
                    cell.Name + ".Value(Formula=" + cell.Formula + ")");
            }
        }
    }
}
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Sets an array formula to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given array formula |

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


