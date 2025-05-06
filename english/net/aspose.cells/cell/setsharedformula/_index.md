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

### Examples

```csharp
// Called: cell.SetSharedFormula(&amp;quot;=C1&amp;quot;, r, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell;
            int r = 500000;
            for (int i = 0; i &lt; r; i++)
            {
                cell = cells[i, 0];
                cell = cells[i, 1];
            }
            cell = cells[0, 0];
            long t = DateTime.Now.ToFileTimeUtc();
            cell.SetSharedFormula(&quot;=C1&quot;, r, 2);
            int c = (int) ((DateTime.Now.ToFileTimeUtc() - t)/1000000);
            t = DateTime.Now.ToFileTimeUtc();
            cell.SetSharedFormula(&quot;=C1&quot;, r, 2);
            int c1 = (int)((DateTime.Now.ToFileTimeUtc() - t) / 1000000);
            string m = &quot;Initial time: &quot; + c/10.0 + &quot;s; Resetting time: &quot; + c1/10.0;
            Console.WriteLine(m);
            if (c1 &gt; (c &lt;&lt; 1))
            {
                Assert.Fail(&quot;Time cost of resetting shared formula exceeded limit! &quot; + m);
            }
        }
```

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


