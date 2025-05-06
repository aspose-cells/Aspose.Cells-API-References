---
title: Cell.SetFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Set the formula and the valuecalculated result of the formula
type: docs
url: /net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| value | Object | The value(calculated result) of the formula. |

### Examples

```csharp
// Called: cells[13, 1].SetFormula(&amp;quot;=B15&amp;quot;, 1);
[Test]
        public void Method_Object_()
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.EnableIterativeCalculation = true;
            wb.Settings.FormulaSettings.MaxIteration = 2;
            wb.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 1].SetFormula(&quot;=B3&quot;, 1);
            cells[1, 1].SetFormula(&quot;=B3&quot;, 1);
            cells[2, 1].SetFormula(&quot;=B4&quot;, 2);
            cells[3, 1].SetFormula(&quot;=B5&quot;, 3);
            cells[4, 1].SetFormula(&quot;=B6+1&quot;, 4);
            cells[5, 1].SetFormula(&quot;=B5&quot;, 4);

            cells[12, 1].SetFormula(&quot;=B12&quot;, 1);
            cells[11, 1].SetFormula(&quot;=B11&quot;, 1);
            cells[10, 1].SetFormula(&quot;=B14&quot;, 1);
            cells[13, 1].SetFormula(&quot;=B15&quot;, 1);
            cells[14, 1].SetFormula(&quot;=B16+1&quot;, 2);
            cells[15, 1].SetFormula(&quot;=B15&quot;, 2);

            cells[20, 1].SetFormula(&quot;=B22+1&quot;, 1);
            cells[21, 1].SetFormula(&quot;=B21&quot;, 1);
            cells[22, 1].SetFormula(&quot;=B21&quot;, 2);
            cells[23, 1].SetFormula(&quot;=B25&quot;, 2);
            cells[24, 1].SetFormula(&quot;=B26&quot;, 2);
            cells[25, 1].SetFormula(&quot;=B21&quot;, 2);
            for (int i = 20; i &lt; 26; i++)
            {
                cells[i, 0].SetFormula(&quot;=B25+B26&quot;, 1);
                cells[i, 2].SetFormula(&quot;=B25+B26&quot;, 1);
            }
            wb.CalculateFormula();
            Assert.AreEqual(3, cells[0, 1].IntValue, &quot;B1 of first calc&quot;);
            Assert.AreEqual(3, cells[1, 1].IntValue, &quot;B2 of first calc&quot;);
            Assert.AreEqual(4, cells[2, 1].IntValue, &quot;B3 of first calc&quot;);
            Assert.AreEqual(5, cells[3, 1].IntValue, &quot;B4 of first calc&quot;);
            Assert.AreEqual(6, cells[4, 1].IntValue, &quot;B5 of first calc&quot;);
            Assert.AreEqual(6, cells[5, 1].IntValue, &quot;B6 of first calc&quot;);
            Assert.AreEqual(2, cells[10, 1].IntValue, &quot;B11 of first calc&quot;);
            Assert.AreEqual(2, cells[11, 1].IntValue, &quot;B12 of first calc&quot;);
            Assert.AreEqual(2, cells[12, 1].IntValue, &quot;B13 of first calc&quot;);
            Assert.AreEqual(3, cells[13, 1].IntValue, &quot;B14 of first calc&quot;);
            Assert.AreEqual(4, cells[14, 1].IntValue, &quot;B15 of first calc&quot;);
            Assert.AreEqual(4, cells[15, 1].IntValue, &quot;B16 of first calc&quot;);
            Assert.AreEqual(3, cells[20, 1].IntValue, &quot;B21 of first calc&quot;);
            Assert.AreEqual(3, cells[21, 1].IntValue, &quot;B22 of first calc&quot;);
            Assert.AreEqual(3, cells[22, 1].IntValue, &quot;B23 of first calc&quot;);
            Assert.AreEqual(2, cells[23, 1].IntValue, &quot;B24 of first calc&quot;);
            Assert.AreEqual(2, cells[24, 1].IntValue, &quot;B25 of first calc&quot;);
            Assert.AreEqual(3, cells[25, 1].IntValue, &quot;B26 of first calc&quot;);
            for (int i = 20; i &lt; 25; i++)
            {
                Assert.AreEqual(4, cells[i, 0].IntValue, &quot;A&quot; + (i + 1) + &quot; of first calc&quot;);
                Assert.AreEqual(4, cells[i, 2].IntValue, &quot;C&quot; + (i + 1) + &quot; of first calc&quot;);
            }
            Assert.AreEqual(4, cells[25, 0].IntValue, &quot;A26 of first calc&quot;);
            Assert.AreEqual(5, cells[25, 2].IntValue, &quot;C26 of first calc&quot;);
            wb.CalculateFormula();
            Assert.AreEqual(5, cells[0, 1].IntValue, &quot;B1 of second calc&quot;);
            Assert.AreEqual(5, cells[1, 1].IntValue, &quot;B2 of second calc&quot;);
            Assert.AreEqual(6, cells[2, 1].IntValue, &quot;B3 of second calc&quot;);
            Assert.AreEqual(7, cells[3, 1].IntValue, &quot;B4 of second calc&quot;);
            Assert.AreEqual(8, cells[4, 1].IntValue, &quot;B5 of second calc&quot;);
            Assert.AreEqual(8, cells[5, 1].IntValue, &quot;B6 of second calc&quot;);
            Assert.AreEqual(4, cells[10, 1].IntValue, &quot;B11 of second calc&quot;);
            Assert.AreEqual(4, cells[11, 1].IntValue, &quot;B12 of second calc&quot;);
            Assert.AreEqual(4, cells[12, 1].IntValue, &quot;B13 of second calc&quot;);
            Assert.AreEqual(5, cells[13, 1].IntValue, &quot;B14 of second calc&quot;);
            Assert.AreEqual(6, cells[14, 1].IntValue, &quot;B15 of second calc&quot;);
            Assert.AreEqual(6, cells[15, 1].IntValue, &quot;B16 of second calc&quot;);
            Assert.AreEqual(5, cells[20, 1].IntValue, &quot;B21 of first calc&quot;);
            Assert.AreEqual(5, cells[21, 1].IntValue, &quot;B22 of first calc&quot;);
            Assert.AreEqual(5, cells[22, 1].IntValue, &quot;B23 of first calc&quot;);
            Assert.AreEqual(3, cells[23, 1].IntValue, &quot;B24 of first calc&quot;);
            Assert.AreEqual(4, cells[24, 1].IntValue, &quot;B25 of first calc&quot;);
            Assert.AreEqual(5, cells[25, 1].IntValue, &quot;B26 of first calc&quot;);
            for (int i = 20; i &lt; 24; i++)
            {
                Assert.AreEqual(7, cells[i, 0].IntValue, &quot;A&quot; + (i + 1) + &quot; of first calc&quot;);
                Assert.AreEqual(7, cells[i, 2].IntValue, &quot;C&quot; + (i + 1) + &quot; of first calc&quot;);
            }
            Assert.AreEqual(7, cells[24, 0].IntValue, &quot;A25 of first calc&quot;);
            Assert.AreEqual(8, cells[24, 2].IntValue, &quot;C25 of first calc&quot;);
            Assert.AreEqual(8, cells[25, 0].IntValue, &quot;A26 of first calc&quot;);
            Assert.AreEqual(9, cells[25, 2].IntValue, &quot;C26 of first calc&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### Examples

```csharp
// Called: cell.SetFormula(fml, po);
[Test]
        public void Method_FormulaParseOptions_()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Cell cell = wb.Worksheets[0].Cells[1, 0];
            Method_FormulaParseOptions_(cell, &quot;=SUM(A1)(B1:B2)&quot;,
                &quot;Non-Reference function cannot be supported to be taken as function name&quot;);
            Method_FormulaParseOptions_(cell, &quot;=RC()&quot;,
                &quot;RC format reference function cannot be supported to be taken as function name&quot;);
            Method_FormulaParseOptions_(cell, &quot;=R1C()&quot;,
                &quot;RC format reference function cannot be supported to be taken as function name&quot;);
            FormulaParseOptions po = new FormulaParseOptions();
            po.R1C1Style = true;
            string fml = &quot;=RC()&quot;;
            cell.SetFormula(fml, po);
            Assert.AreEqual(&quot;=A2()&quot;, cell.Formula, &quot;RC formula: &quot; + fml);
            fml = &quot;=R1C()&quot;;
            cell.SetFormula(fml, po);
            Assert.AreEqual(&quot;=A$1()&quot;, cell.Formula, &quot;RC formula: &quot; + fml);
            fml = &quot;=R()&quot;;
            cell.SetFormula(fml, po);
            Assert.AreEqual(&quot;=2:2()&quot;, cell.Formula, &quot;RC formula: &quot; + fml);

            //CELLSNET-56671
            fml = &quot;=SUM1()&quot;;
            cell.Formula = fml;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;#REF!&quot;, cell.Value, &quot;(Xlsx)Calculated value of: &quot; + fml);
            wb.FileFormat = FileFormatType.Excel97To2003;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;=#REF!()&quot;, cell.Formula, &quot;After converting xlsx to xls: &quot; + fml);
            Assert.AreEqual(&quot;#REF!&quot;, cell.Value, &quot;(Xlsx)Calculated value of: &quot; + fml);
            cell.Formula = fml;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;#NAME?&quot;, cell.Value, &quot;(Xls)Calculated value of: &quot; + fml);
        }
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Set the formula and the value of the formula.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |
| value | Object | The value of the formula. |

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(string,FormulaParseOptions,object). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| value | Object | The value(calculated result) of the formula. |

### Examples

```csharp
// Called: cells[rowIndex, 0].SetFormula(&amp;quot;=1+Sheet1!R[-&amp;quot; + rowIndex + &amp;quot;]C:R[-&amp;quot; + rowIndex
private void Method_Object_(FileFormatType initFft, FileFormatType saveFft)
        {
            //Currently found formulas that are in array formula and have same formula data with ms excel but give different result:
            //  FormulaCalc.xls: INDIRECT(Sheet4!M122,S122), TREND, Operator for different size range, VLOOKUP(Sheet4!I237,I240)
            Workbook wb = new Workbook(initFft);
            wb.Settings.FormulaSettings.PreservePaddingSpaces = true;
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            int rowIndex = 0;
            cells[rowIndex, 0].PutValue(1);
            cells[rowIndex, 1].PutValue(2);
            cells[rowIndex, 2].PutValue(4);
            cells[rowIndex, 3].PutValue(&quot;#VALUE!&quot;);
            cells[rowIndex, 4].PutValue(&quot;#N/A&quot;);
            cells[rowIndex, 5].PutValue(true);
            cells[rowIndex, 6].PutValue(false);
            cells[rowIndex, 7].PutValue(&quot;abc&quot;);
            rowIndex++;
            cells[rowIndex, 0].PutValue(8);
            cells[rowIndex, 1].PutValue(16);
            cells[rowIndex, 2].PutValue(32);
            rowIndex++;
            Util.SetHintMessage(cells[rowIndex, 0],
                &quot;Change cells&apos; value in upper rows, formulas should be recalculated to other valid values.&quot;);

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=RANK.AVG(A1,A1:C1,1)&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=ABS(A1:C1)&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=SUM(ABS(A1:C1))&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=7,\&quot;OK\&quot;,\&quot;Expect 7\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=LOOKUP(A1,ABS(A1:C1))&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;= SUM( IF( NOT( ISERROR( A1: H1 ) ), A1: H1 ), 100 ) &quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=107,\&quot;OK\&quot;,\&quot;Expect 107\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=ISERROR(TREND(A1:B1,,B1:C2))&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect TRUE\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=TREND(A1:B1,,B1:C2)&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=ISERROR(TREND(A1:B1,,B1:C2))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect TRUE\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=TREND(A1:B1,,B1:C2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=ISNA(I1:I3-J1:J2)&quot;, 3, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect FALSE\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect FALSE\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=TRUE,\&quot;OK\&quot;,\&quot;Expect TRUE\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetSharedFormula(&quot;=VLOOKUP(A1,$A$1:$A$2,1,TRUE)&quot;, 2, 2);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=8,\&quot;OK\&quot;,\&quot;Expect 8\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=8,\&quot;OK\&quot;,\&quot;Expect 8\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUMPRODUCT(OFFSET(B3,-2,-1):C1,A2:OFFSET(A1,1,2))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=168,\&quot;OK\&quot;,\&quot;Expect 168\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=ISERROR({1,2,3})&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect FALSE(V)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=ISERROR({1,2,3})&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect FALSE\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM({1;2;3}*{4;5;6})&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=32,\&quot;OK\&quot;,\&quot;Expect 32(AA)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=ABS({1;2;3}*{4;5;6})&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=4,\&quot;OK\&quot;,\&quot;Expect 4(VV)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM({1,2,3}*A1:C1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=6,\&quot;OK\&quot;,\&quot;Expect 6(AV)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=SUM({1,2,3}*A1:C1)&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=17,\&quot;OK\&quot;,\&quot;Expect 17(AA)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=HLOOKUP(2,ABS({1,2,3}),1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=HLOOKUP(2,TREND(A1:B1,B1:C1),1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=HLOOKUP(2,ABS(TREND(A1:B1,B1:C1)),1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM(ABS(TREND(A1:B1,B1:C1)))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=3,\&quot;OK\&quot;,\&quot;Expect 3\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=F1:H1-A1:B1&quot;, 1, 3);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=0,\&quot;OK\&quot;,\&quot;Expect 0\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=-2,\&quot;OK\&quot;,\&quot;Expect -2\&quot;)&quot;;
            //formula data is same with ms excel, maybe caused by other formula options. INDIRECT function seems like this too.
            cells[rowIndex, 6].Formula = &quot;=IF(ISNA(C&quot; + (rowIndex + 1) + &quot;),\&quot;OK\&quot;,\&quot;Expect #N/A but cannot resolved\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=ISERROR(MOD(A1:B1,B1:C1))&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=FALSE,\&quot;OK\&quot;,\&quot;Expect FALSE\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=VLOOKUP(A1:A2,A1:A2,1)&quot;, 2, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=8,\&quot;OK\&quot;,\&quot;Expect 8\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=LOOKUP(2,ABS(IF(A1,{1,2,3},C1:C2)))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2(VAR/AAR)\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=DCOUNTA(A1:H2,{2;8},C1:C2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=DCOUNTA(A1:H2,{2;8},C1:C2)&quot;, 2, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=0,\&quot;OK\&quot;,\&quot;Expect 0\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=TYPE(C1:D1)&quot;, 1, 2);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=64,\&quot;OK\&quot;,\&quot;Expect 64\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=64,\&quot;OK\&quot;,\&quot;Expect 64\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=TYPE(C1)&quot;;
            cells[rowIndex, 1].Formula = &quot;=TYPE(D1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=16,\&quot;OK\&quot;,\&quot;Expect 16\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=TYPE({1,2})&quot;, 1, 2);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=64,\&quot;OK\&quot;,\&quot;Expect 64\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=64,\&quot;OK\&quot;,\&quot;Expect 64\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=TYPE({1,2})&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=64,\&quot;OK\&quot;,\&quot;Expect 64\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=LINEST(A2:B2,A1:B1,TRUE,TRUE)&quot;, 5, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=8,\&quot;OK\&quot;,\&quot;Expect 8\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=0,\&quot;OK\&quot;,\&quot;Expect 0\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            //formula data is same with ms excel, maybe caused by other formula options.
            cells[rowIndex, 4].Formula = &quot;=IF(ISNA(A&quot; + (rowIndex + 1) + &quot;),\&quot;OK\&quot;,\&quot;Expect #N/A but cannot resolved\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=32,\&quot;OK\&quot;,\&quot;Expect 32\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=WORKDAY(A1,1,B1:C1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=3,\&quot;OK\&quot;,\&quot;Expect 3\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=FVSCHEDULE(B1,A1:C1)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=60,\&quot;OK\&quot;,\&quot;Expect 60\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=NETWORKDAYS(2,3,{2,4})&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM(INDEX((A1:A3=8)*(B1:B3=16),0))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula(&quot;=IFERROR(INDEX(A1:A3,1),-1)&quot;, 1, 1); //CELLSNET-46403
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=INDEX(A1:A3,MATCH(8,A1:A3,0))&quot;; //CELLSNET-46430
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=8,\&quot;OK\&quot;,\&quot;Expect 8\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM(IF(FREQUENCY(MATCH(A1:A2,A1:A2,0),MATCH(A1:A2,A1:A2,0))&gt;0,1))&quot;;
            //CELLSNET-45968
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=-B1,C1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=--B1,C1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=--B1,C1-D1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=--B1,C1-D1,D2&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!C1:D1,Sheet1!F1:G1,I1,K1-L1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=-- un an B1,C1-D1,D2&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=5,\&quot;OK\&quot;,\&quot;Expect #NAME?\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=B1:B2()&quot;; //CELLSNET-45968
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=A1:A2(B1:B2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!A1:A2(B1:B2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!A1:Sheet1!A2(B1:B2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=(A1:A2)(B1:B2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=(A1:A2,C2)(B1:B2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            //CELLSNET-56671
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM1()&quot;;
            if (saveFft != FileFormatType.Excel97To2003 || initFft != FileFormatType.Excel97To2003)
            {
                cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            }
            else
            {
                cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=5,\&quot;OK\&quot;,\&quot;Expect #NAME?\&quot;)&quot;;
            }
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=AB()&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=5,\&quot;OK\&quot;,\&quot;Expect #NAME?\&quot;)&quot;;

            //CELLSJAVA-43448
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=test1 -test2 test3, test4&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=5,\&quot;OK\&quot;,\&quot;Expect #NAME?\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=test1-test2/test3^test4/test5,test6/test7+test8,test9&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=5,\&quot;OK\&quot;,\&quot;Expect #NAME?\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=(A1/A2,A2/3)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=-A1^A2,A3&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=A1-A2,A3&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=---A2,A3+---A4,A5&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=3,\&quot;OK\&quot;,\&quot;Expect #VALUE!\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=INDIRECT(A1)(B1:B2,C3,D2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!$A$1%&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(A&quot; + (rowIndex + 1) + &quot;=0.01,\&quot;OK\&quot;,\&quot;Expect 0.01\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!$A$1 %&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(A&quot; + (rowIndex + 1) + &quot;=0.01,\&quot;OK\&quot;,\&quot;Expect 0.01\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=Sheet1!$A$1:$C$1%&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(A&quot; + (rowIndex + 1) + &quot;=0.01,\&quot;OK\&quot;,\&quot;Expect 0.01\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=1+Sheet1!$A$1:$B$1 Sheet1!$B$1:$C$1%&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(A&quot; + (rowIndex + 1) + &quot;=1.02,\&quot;OK\&quot;,\&quot;Expect 1.02\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].SetFormula(&quot;=1+Sheet1!R[-&quot; + rowIndex + &quot;]C:R[-&quot; + rowIndex
                + &quot;]C[1] Sheet1!R[-&quot; + rowIndex + &quot;]C[1]:R[-&quot; + rowIndex + &quot;]C[2]%&quot;,
                new FormulaParseOptions(){R1C1Style = true}, null);
            cells[rowIndex, 4].Formula = &quot;=IF(A&quot; + (rowIndex + 1) + &quot;=1.02,\&quot;OK\&quot;,\&quot;Expect 1.02\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].R1C1Formula = &quot;=SUM(R1C[+1]:R1C[+2])&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,0)=6,\&quot;OK\&quot;,\&quot;Expect 6\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUMPRODUCT(SUBTOTAL(4,OFFSET(Sheet1!$A$1:$B$1,0,COLUMN(Sheet1!$A$1:$B$1)-1)),Sheet1!$A$2:$B$2)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=80,\&quot;OK\&quot;,\&quot;Expect 80\&quot;)&quot;;

            rowIndex++; //CELLSNET-46994
            cells[rowIndex, 0].Formula = &quot;=IF($A$1=-1,0,IF($A$1=-2,0,SUMIF(Sheet1!$A$1:$A$2,$A$1,Sheet1!$C$1:$C$2)))&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=4,\&quot;OK\&quot;,\&quot;Expect 4\&quot;)&quot;;

            rowIndex++; //CELLSNET-47007
            cells[rowIndex, 0].Formula = &quot;=IFERROR(MATCH($A$1,$A$1:$A$3,0),\&quot;Incorrectly parsed formula\&quot;)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;

            rowIndex++; //CELLSNET-47029
            cells[rowIndex, 0].Formula = &quot;=SUMPRODUCT(MAX($A$1:$A$3=1))+1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUMPRODUCT(MAX($A$1:$A$3=1)*1)+1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=1,\&quot;OK\&quot;,\&quot;Expect 1\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUMPRODUCT(MAX(($A$1:$A$3=1)*1))+1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=IF(AND(INDEX($A$1:$A$3,1,MATCH($A$1,$A$1:$A$3))=1,2),3,4)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=3,\&quot;OK\&quot;,\&quot;Expect 3\&quot;)&quot;;

            rowIndex++; //CELLSPYTHONJAVA-89
            cells[rowIndex, 2].SetDynamicArrayFormula(&quot;=\&quot;\&quot;&quot;, new FormulaParseOptions(), true);
            cells[rowIndex, 3].SetDynamicArrayFormula(&quot;=\&quot;\&quot;&quot;, new FormulaParseOptions(), true);
            cells[rowIndex, 0].SetSharedFormula(&quot;=AVERAGE(C&quot; + (rowIndex + 1) + &quot;#)&quot;, 1, 2);
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=2,\&quot;OK\&quot;,\&quot;Expect #DIV/0!\&quot;)&quot;;

            NameCollection names = wb.Worksheets.Names;
            Name name = names[names.Add(&quot;TestNameCommon&quot;)];
            name.RefersTo = &quot;=Sheet1!$A$1:$C$1&quot;;
            rowIndex++; //Name for CELLSNET-47118, @ for 47251
            cells[rowIndex, 0].SetArrayFormula(&quot;=@INDEX($A$2:$C$2,1,MATCH(1,TestNameCommon-1,0))&quot;, 1, 1);
            cells[rowIndex, 1].SetArrayFormula(&quot;=INDEX($A$2:$C$2,1,MATCH(1,$A$1:$C$1-1,0))&quot;, 1, 1);
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=16,\&quot;OK\&quot;,\&quot;Expect 16\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=16,\&quot;OK\&quot;,\&quot;Expect 16\&quot;)&quot;;

            name = names[names.Add(&quot;TestNameRelative&quot;)];
            name.RefersTo = &quot;=SUM(A$1:A$2)&quot;;
            Assert.AreEqual(&quot;=SUM(!A$1:A$2)&quot;, name.RefersTo, &quot;Relative reference in Name.RefersTo&quot;);
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=TestNameRelative&quot;;
            cells[rowIndex, 1].Formula = &quot;=TestNameRelative&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,0)=9,\&quot;OK\&quot;,\&quot;Expect 9\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,0)=18,\&quot;OK\&quot;,\&quot;Expect 18\&quot;)&quot;;

            //CELLSNET-52858: AddIn functions cannot be converted correctly from xlsx to xls, generate corrupted file
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=GCD(5000,5100)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,0)=100,\&quot;OK\&quot;,\&quot;Expect 100\&quot;)&quot;;

            //CELLSJAVA-43219: sheet reference without quote caused corrupted file
            Worksheet specialSheet = wb.Worksheets.Add(&quot;a12345.b67890.&quot;);
            specialSheet.Cells[0, 0].PutValue(1);
            specialSheet.IsVisible = false;
            specialSheet = wb.Worksheets.Add(&quot;. special&quot;);
            specialSheet.Cells[0, 0].PutValue(2);
            specialSheet.IsVisible = false;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=&apos;a12345.b67890.&apos;!A1+1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=2,\&quot;OK\&quot;,\&quot;Expect 2\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=&apos;. special&apos;!A1+1&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=3,\&quot;OK\&quot;,\&quot;Expect 3\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=A1:B1\n   B1:B2&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=A1:B1\&quot;&amp;CHAR(10)&amp;\&quot;   B1:B2\&quot;,\&quot;OK\&quot;,\&quot;Incorrect linebreak and space in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=B1:B2  #REF!&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=B1:B2  #REF!\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=INDIRECT(  \&quot;B1\&quot;,   TRUE    )&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=INDIRECT(  \&quot;\&quot;B1\&quot;\&quot;,   TRUE    )\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= IF(  FALSE,   1,    2     )&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= IF(  FALSE,   1,    2     )\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=IF(B1 &lt;&gt;0,1,0)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=IF(B1 &lt;&gt;0,1,0)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=IF(B1&lt;&gt; 0,1,0)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=IF(B1&lt;&gt; 0,1,0)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=1+\n((2/3)*5)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=1+\&quot;&amp;CHAR(10)&amp;\&quot;((2/3)*5)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=IF(A4&gt;0,A4 &amp; &apos;. special&apos;!A4)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;=IF(A4&gt;0,A4 &amp; &apos;. special&apos;!A4)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= CHOOSE(  1,   1,    2     )&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= CHOOSE(  1,   1,    2     )\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= NUMBERVALUE(\&quot;01:02\&quot;)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= NUMBERVALUE(\&quot;\&quot;01:02\&quot;\&quot;)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= NUMBERVALUE(\&quot;01:02\&quot;,\&quot;.\&quot;)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= NUMBERVALUE(\&quot;\&quot;01:02\&quot;\&quot;,\&quot;\&quot;.\&quot;\&quot;)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= NUMBERVALUE(\&quot;01:02\&quot;,\&quot;.\&quot;,\&quot;;\&quot;)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= NUMBERVALUE(\&quot;\&quot;01:02\&quot;\&quot;,\&quot;\&quot;.\&quot;\&quot;,\&quot;\&quot;;\&quot;\&quot;)\&quot;,\&quot;OK\&quot;,\&quot;Incorrect spaces in formula\&quot;)&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;= 1  +\n   (    2     +      3       )        +\n         RAND()&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(SUBSTITUTE(FORMULATEXT(A&quot;
                + (rowIndex + 1) + &quot;),\&quot;@\&quot;,\&quot;\&quot;)=\&quot;= 1  +\&quot;&amp;CHAR(10)&amp;\&quot;   (    2     +      3       )        +\&quot;&amp;CHAR(10)&amp;\&quot;         RAND()\&quot;,\&quot;OK\&quot;,\&quot;Incorrect linebreak and space in formula\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=ROWS($B$1+$C$1:$C$3)&quot;; //CELLSNET-56016
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=3,\&quot;OK\&quot;,\&quot;Expect 3\&quot;)&quot;;

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM(XLOOKUP(1,A1:A3,C1:C3):XLOOKUP(8,A2,B2))&quot;; //CELLSNET-56879
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=54,\&quot;OK\&quot;,\&quot;Expect 54\&quot;)&quot;;

            name = names[names.Add(&quot;TestNameOperator&quot;)];
            name.RefersTo = &quot;=Sheet1!$A$1:A$2+Sheet1!$B$1:B$2&quot;;
            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=SUM(TestNameOperator)&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,\&quot;Error\&quot;)=27,\&quot;OK\&quot;,\&quot;Expect 27\&quot;)&quot;;


            cells = wb.Worksheets.Add(&quot;AnotherSheet&quot;).Cells;
            rowIndex = 0;
            cells[rowIndex, 0].PutValue(128);
            cells[rowIndex, 1].PutValue(256);
            cells[rowIndex, 2].PutValue(512);
            rowIndex++;
            cells[rowIndex, 0].PutValue(1024);
            cells[rowIndex, 1].PutValue(2048);
            cells[rowIndex, 2].PutValue(4096);
            rowIndex++;
            Util.SetHintMessage(cells[rowIndex, 0],
                &quot;Change cells&apos; value in upper rows, formulas should be recalculated to other valid values.&quot;);

            rowIndex++;
            cells[rowIndex, 0].Formula = &quot;=TestNameRelative&quot;;
            cells[rowIndex, 1].Formula = &quot;=TestNameRelative&quot;;
            cells[rowIndex, 4].Formula = &quot;=IF(IFERROR(A&quot; + (rowIndex + 1) + &quot;,0)=1152,\&quot;OK\&quot;,\&quot;Expect 1152\&quot;)&quot;;
            cells[rowIndex, 5].Formula = &quot;=IF(IFERROR(B&quot; + (rowIndex + 1) + &quot;,0)=2304,\&quot;OK\&quot;,\&quot;Expect 2304\&quot;)&quot;;

            //CELLSNET-56588
            sheet = wb.Worksheets.Add(&quot;Others&quot;);
            cells = sheet.Cells;
            Util.SetHintMessage(cells[0, 0], &quot;Only A4 should be filled with red color for conditional formatting.&quot;);
            rowIndex = 1;
            cells[rowIndex++, 0].PutValue(0);
            cells[rowIndex++, 0].PutValue(1);
            cells[rowIndex++, 0].PutValue(2);
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.Add(CellArea.CreateCellArea(1, 0, 3, 0), FormatConditionType.Expression, OperatorType.None,
                &quot;=A2&gt;AVERAGE($A$2:$A$4-0)&quot;, null);
            fcc[0].Style.Pattern = BackgroundType.Solid;
            fcc[0].Style.BackgroundColor = Color.Red;

            //CELLSNET-56624,CELLSJAVA-46108
            rowIndex += 2;
            Util.SetHintMessage(cells[rowIndex, 0], &quot;Press on this cell, cell name should be replaced to ReplacedCellName.&quot;);
            name = names[names.Add(&quot;ReplacedCellName&quot;)];
            name.RefersTo = &quot;=Others!$A$&quot; + (rowIndex + 1);

            //CELLSNODEJSCPP-46: name formula without mem becomes invalid and cause file corrupted
            name = names[names.Add(&quot;InvalidRefNeedMem1&quot;)];
            name.RefersTo = &quot;#REF!,Sheet1!$A$1&quot;;
            name = names[names.Add(&quot;InvalidRefNeedMem2&quot;)];
            name.RefersTo = &quot;#REF!,#REF!,#REF!&quot;;
            rowIndex += 2;
            cells[rowIndex++, 0].Formula = &quot;#REF!,#REF!,#REF!&quot;; //it is ok even without mem
            cells[rowIndex, 0].Formula = &quot;InvalidRefNeedMem1&quot;; //it is ok even without mem
            cells[rowIndex, 4].Formula = &quot;=IF(ERROR.TYPE(A&quot; + (rowIndex + 1) + &quot;)=4,\&quot;OK\&quot;,\&quot;Expect #REF!\&quot;)&quot;;

            if (initFft != FileFormatType.Excel97To2003 &amp;&amp; saveFft != FileFormatType.Excel97To2003)
	        {
                sheet = wb.Worksheets.Add(&quot;TableRefences&quot;);
                cells = sheet.Cells;
                cells[0, 0].PutValue(&quot;#Column1&quot;);
                cells[0, 1].PutValue(&quot;@Column2&quot;);
                cells[0, 2].PutValue(&quot;[Column3&quot;);
                cells[0, 3].PutValue(&quot;]Column4&quot;);
                cells[0, 4].PutValue(&quot;&amp;C o#l@u[m]n&apos;5\&quot;&quot;);
                for (int i = 1; i &lt; 4; i++)
                {
                    for (int j = 0; j &lt; 5; j++)
                    {
                        cells[i, j].PutValue(i * 5 + j);
                    }
                }
                sheet.ListObjects.Add(0, 0, 3, 4, true);
                ListObject list = sheet.ListObjects[0];
                list.ShowTotals = true;
                list.DisplayName = &quot;TestTable1&quot;;
                cells[2, 6].Formula = &quot;=SUM(TestTable1[&apos;@Column2])&quot;;
                cells[2, 7].Formula = &quot;=SUM(TestTable1[@[&apos;@Column2]:[&amp;C o&apos;#l&apos;@u&apos;[m&apos;]n&apos;&apos;5\&quot;]])&quot;;
                cells[3, 0].Formula = &quot;SUM([@&amp;C o&apos;#l&apos;@u&apos;[m&apos;]n&apos;&apos;5\&quot;])&quot;;
                cells[5, 0].Formula = &quot;SUM(TestTable1[ [&apos;#Column1] ])&quot;;
                cells[5, 1].Formula = &quot;SUM(TestTable1[ [#Totals],[&apos;#Column1]])&quot;;
                cells[5, 2].Formula = &quot;SUM(TestTable1[[#Totals],[&apos;#Column1]:[&apos;@Column2]])&quot;;
                cells[5, 3].Formula = &quot;SUM(TestTable1[ [&apos;[Column3]:[&apos;]Column4]])&quot;;
                cells[6, 0].Formula = &quot;SUM(externalbook.xlsx!TestTable1[[#Totals],[&apos;[Column3]:[&apos;]Column4]])&quot;;
                //CELLSNET-47872
                cells[6, 1].Formula = &quot;VLOOKUP(\&quot;Total\&quot;,TestTable1[[#Data],[#Totals]],5,FALSE)&quot;;
                Assert.AreEqual(&quot;=VLOOKUP(\&quot;Total\&quot;,TestTable1[[#Data],[#Totals]],5,FALSE)&quot;, cells[6, 1].Formula);
                cells[6, 2].Formula = &quot;VLOOKUP(\&quot;#Column1\&quot;,TestTable1[[#Headers],[#Data]],2,FALSE)&quot;;
                Assert.AreEqual(&quot;=VLOOKUP(\&quot;#Column1\&quot;,TestTable1[[#Headers],[#Data]],2,FALSE)&quot;, cells[6, 2].Formula);
            }
            if (saveFft != initFft)
            {
                Util.SaveManCheck(wb, &quot;Formula&quot;, &quot;Parser_&quot;
                    + Util.GetFileExt(initFft) + &quot;.&quot; + Util.GetFileExt(saveFft));
            }
            else
            {
                Util.SaveManCheck(wb, &quot;Formula&quot;, &quot;Parser.&quot; + Util.GetFileExt(saveFft));
            }
        }
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


