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
// Called: cells[0, 0].SetFormula("=MYFUNC()", "OriginalValue");
[Test]
        public void Method_Object_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetFormula("=MYFUNC()", "OriginalValue");
            cells[0, 1].SetFormula("=SUM(1,2)", 4);
            wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomEnginJ45190(null) });
            Assert.AreEqual("OriginalValue", cells[0, 0].StringValue, "IgnoreCalculatingCustomFunction: MYFUNC");
            Assert.AreEqual(4, cells[0, 1].IntValue, "IgnoreCalculatingCustomFunction: SUM");
            object[] buffer = new object[2];
            wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomEnginJ45190(buffer) });
            Assert.AreEqual("#NAME?", buffer[0], "CallBuiltInEngine: MYFUNC");
            Assert.AreEqual(3, buffer[1], "CallBuiltInEngine: SUM");
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
// Called: cells[1, c2++].SetFormula("=TEST_UDF()", new FormulaParseOptions());
[Test]
        public void Method_FormulaParseOptions_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            int c1 = 0;
            int c2 = 0;
            cells[0, c1++].Formula = "=TEST_UDF()";
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);
            cells[1, c2++].Formula = "=Test.xlam!TEST_UDF()";
            cells[1, c2++].Formula = "=TEST_UDF()";
            cells[1, c2++].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            cells[0, c1++].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false }, null);
            for (c1--; c1 > -1; c1--)
            {
                Assert.AreEqual("=TEST_UDF()", cells[0, c1].Formula, CellsHelper.CellIndexToName(0, c1));
            }
            for (c2--; c2 > -1; c2--)
            {
                Assert.AreEqual("=Test.xlam!TEST_UDF()", cells[1, c2].Formula, CellsHelper.CellIndexToName(1, c2));
            }
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
// Called: cells[rowIndex, 0].SetFormula("=1+Sheet1!R[-" + rowIndex + "]C:R[-" + rowIndex
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
            cells[rowIndex, 3].PutValue("#VALUE!");
            cells[rowIndex, 4].PutValue("#N/A");
            cells[rowIndex, 5].PutValue(true);
            cells[rowIndex, 6].PutValue(false);
            cells[rowIndex, 7].PutValue("abc");
            rowIndex++;
            cells[rowIndex, 0].PutValue(8);
            cells[rowIndex, 1].PutValue(16);
            cells[rowIndex, 2].PutValue(32);
            rowIndex++;
            Util.SetHintMessage(cells[rowIndex, 0],
                "Change cells' value in upper rows, formulas should be recalculated to other valid values.");

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=RANK.AVG(A1,A1:C1,1)", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=ABS(A1:C1)", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=SUM(ABS(A1:C1))", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=7,\"OK\",\"Expect 7\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=LOOKUP(A1,ABS(A1:C1))", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("= SUM( IF( NOT( ISERROR( A1: H1 ) ), A1: H1 ), 100 ) ", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=107,\"OK\",\"Expect 107\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=ISERROR(TREND(A1:B1,,B1:C2))", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect TRUE\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=TREND(A1:B1,,B1:C2)", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=ISERROR(TREND(A1:B1,,B1:C2))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect TRUE\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=TREND(A1:B1,,B1:C2)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=ISNA(I1:I3-J1:J2)", 3, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect FALSE\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect FALSE\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=TRUE,\"OK\",\"Expect TRUE\")";

            rowIndex++;
            cells[rowIndex, 0].SetSharedFormula("=VLOOKUP(A1,$A$1:$A$2,1,TRUE)", 2, 2);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=8,\"OK\",\"Expect 8\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=8,\"OK\",\"Expect 8\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUMPRODUCT(OFFSET(B3,-2,-1):C1,A2:OFFSET(A1,1,2))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=168,\"OK\",\"Expect 168\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=ISERROR({1,2,3})";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect FALSE(V)\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=ISERROR({1,2,3})", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect FALSE\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM({1;2;3}*{4;5;6})";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=32,\"OK\",\"Expect 32(AA)\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=ABS({1;2;3}*{4;5;6})";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=4,\"OK\",\"Expect 4(VV)\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM({1,2,3}*A1:C1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=6,\"OK\",\"Expect 6(AV)\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=SUM({1,2,3}*A1:C1)", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=17,\"OK\",\"Expect 17(AA)\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=HLOOKUP(2,ABS({1,2,3}),1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=HLOOKUP(2,TREND(A1:B1,B1:C1),1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=HLOOKUP(2,ABS(TREND(A1:B1,B1:C1)),1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM(ABS(TREND(A1:B1,B1:C1)))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=3,\"OK\",\"Expect 3\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=F1:H1-A1:B1", 1, 3);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=0,\"OK\",\"Expect 0\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=-2,\"OK\",\"Expect -2\")";
            //formula data is same with ms excel, maybe caused by other formula options. INDIRECT function seems like this too.
            cells[rowIndex, 6].Formula = "=IF(ISNA(C" + (rowIndex + 1) + "),\"OK\",\"Expect #N/A but cannot resolved\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=ISERROR(MOD(A1:B1,B1:C1))", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=FALSE,\"OK\",\"Expect FALSE\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=VLOOKUP(A1:A2,A1:A2,1)", 2, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=8,\"OK\",\"Expect 8\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=LOOKUP(2,ABS(IF(A1,{1,2,3},C1:C2)))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2(VAR/AAR)\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=DCOUNTA(A1:H2,{2;8},C1:C2)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=DCOUNTA(A1:H2,{2;8},C1:C2)", 2, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=0,\"OK\",\"Expect 0\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=TYPE(C1:D1)", 1, 2);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=64,\"OK\",\"Expect 64\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=64,\"OK\",\"Expect 64\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=TYPE(C1)";
            cells[rowIndex, 1].Formula = "=TYPE(D1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=16,\"OK\",\"Expect 16\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=TYPE({1,2})", 1, 2);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=64,\"OK\",\"Expect 64\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=64,\"OK\",\"Expect 64\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=TYPE({1,2})";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=64,\"OK\",\"Expect 64\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=LINEST(A2:B2,A1:B1,TRUE,TRUE)", 5, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=8,\"OK\",\"Expect 8\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=0,\"OK\",\"Expect 0\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            //formula data is same with ms excel, maybe caused by other formula options.
            cells[rowIndex, 4].Formula = "=IF(ISNA(A" + (rowIndex + 1) + "),\"OK\",\"Expect #N/A but cannot resolved\")";
            rowIndex++;
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=32,\"OK\",\"Expect 32\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=WORKDAY(A1,1,B1:C1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=3,\"OK\",\"Expect 3\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=FVSCHEDULE(B1,A1:C1)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=60,\"OK\",\"Expect 60\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=NETWORKDAYS(2,3,{2,4})";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM(INDEX((A1:A3=8)*(B1:B3=16),0))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++;
            cells[rowIndex, 0].SetArrayFormula("=IFERROR(INDEX(A1:A3,1),-1)", 1, 1); //CELLSNET-46403
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=INDEX(A1:A3,MATCH(8,A1:A3,0))"; //CELLSNET-46430
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=8,\"OK\",\"Expect 8\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM(IF(FREQUENCY(MATCH(A1:A2,A1:A2,0),MATCH(A1:A2,A1:A2,0))>0,1))";
            //CELLSNET-45968
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=-B1,C1";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=--B1,C1";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=--B1,C1-D1";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=--B1,C1-D1,D2";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!C1:D1,Sheet1!F1:G1,I1,K1-L1";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=-- un an B1,C1-D1,D2";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=5,\"OK\",\"Expect #NAME?\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=B1:B2()"; //CELLSNET-45968
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=A1:A2(B1:B2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!A1:A2(B1:B2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!A1:Sheet1!A2(B1:B2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=(A1:A2)(B1:B2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=(A1:A2,C2)(B1:B2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            //CELLSNET-56671
            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM1()";
            if (saveFft != FileFormatType.Excel97To2003 || initFft != FileFormatType.Excel97To2003)
            {
                cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            }
            else
            {
                cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=5,\"OK\",\"Expect #NAME?\")";
            }
            rowIndex++;
            cells[rowIndex, 0].Formula = "=AB()";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=5,\"OK\",\"Expect #NAME?\")";

            //CELLSJAVA-43448
            rowIndex++;
            cells[rowIndex, 0].Formula = "=test1 -test2 test3, test4";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=5,\"OK\",\"Expect #NAME?\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=test1-test2/test3^test4/test5,test6/test7+test8,test9";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=5,\"OK\",\"Expect #NAME?\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=(A1/A2,A2/3)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=-A1^A2,A3";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=A1-A2,A3";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=---A2,A3+---A4,A5";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=3,\"OK\",\"Expect #VALUE!\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=INDIRECT(A1)(B1:B2,C3,D2)";
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!$A$1%";
            cells[rowIndex, 4].Formula = "=IF(A" + (rowIndex + 1) + "=0.01,\"OK\",\"Expect 0.01\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!$A$1 %";
            cells[rowIndex, 4].Formula = "=IF(A" + (rowIndex + 1) + "=0.01,\"OK\",\"Expect 0.01\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=Sheet1!$A$1:$C$1%";
            cells[rowIndex, 4].Formula = "=IF(A" + (rowIndex + 1) + "=0.01,\"OK\",\"Expect 0.01\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=1+Sheet1!$A$1:$B$1 Sheet1!$B$1:$C$1%";
            cells[rowIndex, 4].Formula = "=IF(A" + (rowIndex + 1) + "=1.02,\"OK\",\"Expect 1.02\")";
            rowIndex++;
            cells[rowIndex, 0].SetFormula("=1+Sheet1!R[-" + rowIndex + "]C:R[-" + rowIndex
                + "]C[1] Sheet1!R[-" + rowIndex + "]C[1]:R[-" + rowIndex + "]C[2]%",
                new FormulaParseOptions(){R1C1Style = true}, null);
            cells[rowIndex, 4].Formula = "=IF(A" + (rowIndex + 1) + "=1.02,\"OK\",\"Expect 1.02\")";
            rowIndex++;
            cells[rowIndex, 0].R1C1Formula = "=SUM(R1C[+1]:R1C[+2])";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",0)=6,\"OK\",\"Expect 6\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUMPRODUCT(SUBTOTAL(4,OFFSET(Sheet1!$A$1:$B$1,0,COLUMN(Sheet1!$A$1:$B$1)-1)),Sheet1!$A$2:$B$2)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=80,\"OK\",\"Expect 80\")";

            rowIndex++; //CELLSNET-46994
            cells[rowIndex, 0].Formula = "=IF($A$1=-1,0,IF($A$1=-2,0,SUMIF(Sheet1!$A$1:$A$2,$A$1,Sheet1!$C$1:$C$2)))";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=4,\"OK\",\"Expect 4\")";

            rowIndex++; //CELLSNET-47007
            cells[rowIndex, 0].Formula = "=IFERROR(MATCH($A$1,$A$1:$A$3,0),\"Incorrectly parsed formula\")";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";

            rowIndex++; //CELLSNET-47029
            cells[rowIndex, 0].Formula = "=SUMPRODUCT(MAX($A$1:$A$3=1))+1";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUMPRODUCT(MAX($A$1:$A$3=1)*1)+1";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=1,\"OK\",\"Expect 1\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUMPRODUCT(MAX(($A$1:$A$3=1)*1))+1";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=IF(AND(INDEX($A$1:$A$3,1,MATCH($A$1,$A$1:$A$3))=1,2),3,4)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=3,\"OK\",\"Expect 3\")";

            rowIndex++; //CELLSPYTHONJAVA-89
            cells[rowIndex, 2].SetDynamicArrayFormula("=\"\"", new FormulaParseOptions(), true);
            cells[rowIndex, 3].SetDynamicArrayFormula("=\"\"", new FormulaParseOptions(), true);
            cells[rowIndex, 0].SetSharedFormula("=AVERAGE(C" + (rowIndex + 1) + "#)", 1, 2);
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=2,\"OK\",\"Expect #DIV/0!\")";

            NameCollection names = wb.Worksheets.Names;
            Name name = names[names.Add("TestNameCommon")];
            name.RefersTo = "=Sheet1!$A$1:$C$1";
            rowIndex++; //Name for CELLSNET-47118, @ for 47251
            cells[rowIndex, 0].SetArrayFormula("=@INDEX($A$2:$C$2,1,MATCH(1,TestNameCommon-1,0))", 1, 1);
            cells[rowIndex, 1].SetArrayFormula("=INDEX($A$2:$C$2,1,MATCH(1,$A$1:$C$1-1,0))", 1, 1);
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=16,\"OK\",\"Expect 16\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",\"Error\")=16,\"OK\",\"Expect 16\")";

            name = names[names.Add("TestNameRelative")];
            name.RefersTo = "=SUM(A$1:A$2)";
            Assert.AreEqual("=SUM(!A$1:A$2)", name.RefersTo, "Relative reference in Name.RefersTo");
            rowIndex++;
            cells[rowIndex, 0].Formula = "=TestNameRelative";
            cells[rowIndex, 1].Formula = "=TestNameRelative";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",0)=9,\"OK\",\"Expect 9\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",0)=18,\"OK\",\"Expect 18\")";

            //CELLSNET-52858: AddIn functions cannot be converted correctly from xlsx to xls, generate corrupted file
            rowIndex++;
            cells[rowIndex, 0].Formula = "=GCD(5000,5100)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",0)=100,\"OK\",\"Expect 100\")";

            //CELLSJAVA-43219: sheet reference without quote caused corrupted file
            Worksheet specialSheet = wb.Worksheets.Add("a12345.b67890.");
            specialSheet.Cells[0, 0].PutValue(1);
            specialSheet.IsVisible = false;
            specialSheet = wb.Worksheets.Add(". special");
            specialSheet.Cells[0, 0].PutValue(2);
            specialSheet.IsVisible = false;
            rowIndex++;
            cells[rowIndex, 0].Formula = "='a12345.b67890.'!A1+1";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=2,\"OK\",\"Expect 2\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "='. special'!A1+1";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=3,\"OK\",\"Expect 3\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=A1:B1\n   B1:B2";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=A1:B1\"&CHAR(10)&\"   B1:B2\",\"OK\",\"Incorrect linebreak and space in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=B1:B2  #REF!";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=B1:B2  #REF!\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=INDIRECT(  \"B1\",   TRUE    )";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=INDIRECT(  \"\"B1\"\",   TRUE    )\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= IF(  FALSE,   1,    2     )";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= IF(  FALSE,   1,    2     )\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=IF(B1 <>0,1,0)";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=IF(B1 <>0,1,0)\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=IF(B1<> 0,1,0)";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=IF(B1<> 0,1,0)\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=1+\n((2/3)*5)";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=1+\"&CHAR(10)&\"((2/3)*5)\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=IF(A4>0,A4 & '. special'!A4)";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"=IF(A4>0,A4 & '. special'!A4)\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= CHOOSE(  1,   1,    2     )";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= CHOOSE(  1,   1,    2     )\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= NUMBERVALUE(\"01:02\")";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= NUMBERVALUE(\"\"01:02\"\")\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= NUMBERVALUE(\"01:02\",\".\")";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= NUMBERVALUE(\"\"01:02\"\",\"\".\"\")\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= NUMBERVALUE(\"01:02\",\".\",\";\")";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= NUMBERVALUE(\"\"01:02\"\",\"\".\"\",\"\";\"\")\",\"OK\",\"Incorrect spaces in formula\")";
            rowIndex++;
            cells[rowIndex, 0].Formula = "= 1  +\n   (    2     +      3       )        +\n         RAND()";
            cells[rowIndex, 4].Formula = "=IF(SUBSTITUTE(FORMULATEXT(A"
                + (rowIndex + 1) + "),\"@\",\"\")=\"= 1  +\"&CHAR(10)&\"   (    2     +      3       )        +\"&CHAR(10)&\"         RAND()\",\"OK\",\"Incorrect linebreak and space in formula\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=ROWS($B$1+$C$1:$C$3)"; //CELLSNET-56016
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=3,\"OK\",\"Expect 3\")";

            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM(XLOOKUP(1,A1:A3,C1:C3):XLOOKUP(8,A2,B2))"; //CELLSNET-56879
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=54,\"OK\",\"Expect 54\")";

            name = names[names.Add("TestNameOperator")];
            name.RefersTo = "=Sheet1!$A$1:A$2+Sheet1!$B$1:B$2";
            rowIndex++;
            cells[rowIndex, 0].Formula = "=SUM(TestNameOperator)";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",\"Error\")=27,\"OK\",\"Expect 27\")";


            cells = wb.Worksheets.Add("AnotherSheet").Cells;
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
                "Change cells' value in upper rows, formulas should be recalculated to other valid values.");

            rowIndex++;
            cells[rowIndex, 0].Formula = "=TestNameRelative";
            cells[rowIndex, 1].Formula = "=TestNameRelative";
            cells[rowIndex, 4].Formula = "=IF(IFERROR(A" + (rowIndex + 1) + ",0)=1152,\"OK\",\"Expect 1152\")";
            cells[rowIndex, 5].Formula = "=IF(IFERROR(B" + (rowIndex + 1) + ",0)=2304,\"OK\",\"Expect 2304\")";

            //CELLSNET-56588
            sheet = wb.Worksheets.Add("Others");
            cells = sheet.Cells;
            Util.SetHintMessage(cells[0, 0], "Only A4 should be filled with red color for conditional formatting.");
            rowIndex = 1;
            cells[rowIndex++, 0].PutValue(0);
            cells[rowIndex++, 0].PutValue(1);
            cells[rowIndex++, 0].PutValue(2);
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.Add(CellArea.CreateCellArea(1, 0, 3, 0), FormatConditionType.Expression, OperatorType.None,
                "=A2>AVERAGE($A$2:$A$4-0)", null);
            fcc[0].Style.Pattern = BackgroundType.Solid;
            fcc[0].Style.BackgroundColor = Color.Red;

            //CELLSNET-56624,CELLSJAVA-46108
            rowIndex += 2;
            Util.SetHintMessage(cells[rowIndex, 0], "Press on this cell, cell name should be replaced to ReplacedCellName.");
            name = names[names.Add("ReplacedCellName")];
            name.RefersTo = "=Others!$A$" + (rowIndex + 1);

            //CELLSNODEJSCPP-46: name formula without mem becomes invalid and cause file corrupted
            name = names[names.Add("InvalidRefNeedMem1")];
            name.RefersTo = "#REF!,Sheet1!$A$1";
            name = names[names.Add("InvalidRefNeedMem2")];
            name.RefersTo = "#REF!,#REF!,#REF!";
            rowIndex += 2;
            cells[rowIndex++, 0].Formula = "#REF!,#REF!,#REF!"; //it is ok even without mem
            cells[rowIndex, 0].Formula = "InvalidRefNeedMem1"; //it is ok even without mem
            cells[rowIndex, 4].Formula = "=IF(ERROR.TYPE(A" + (rowIndex + 1) + ")=4,\"OK\",\"Expect #REF!\")";

            if (initFft != FileFormatType.Excel97To2003 && saveFft != FileFormatType.Excel97To2003)
	        {
                sheet = wb.Worksheets.Add("TableRefences");
                cells = sheet.Cells;
                cells[0, 0].PutValue("#Column1");
                cells[0, 1].PutValue("@Column2");
                cells[0, 2].PutValue("[Column3");
                cells[0, 3].PutValue("]Column4");
                cells[0, 4].PutValue("&C o#l@u[m]n'5\"");
                for (int i = 1; i < 4; i++)
                {
                    for (int j = 0; j < 5; j++)
                    {
                        cells[i, j].PutValue(i * 5 + j);
                    }
                }
                sheet.ListObjects.Add(0, 0, 3, 4, true);
                ListObject list = sheet.ListObjects[0];
                list.ShowTotals = true;
                list.DisplayName = "TestTable1";
                cells[2, 6].Formula = "=SUM(TestTable1['@Column2])";
                cells[2, 7].Formula = "=SUM(TestTable1[@['@Column2]:[&C o'#l'@u'[m']n''5\"]])";
                cells[3, 0].Formula = "SUM([@&C o'#l'@u'[m']n''5\"])";
                cells[5, 0].Formula = "SUM(TestTable1[ ['#Column1] ])";
                cells[5, 1].Formula = "SUM(TestTable1[ [#Totals],['#Column1]])";
                cells[5, 2].Formula = "SUM(TestTable1[[#Totals],['#Column1]:['@Column2]])";
                cells[5, 3].Formula = "SUM(TestTable1[ ['[Column3]:[']Column4]])";
                cells[6, 0].Formula = "SUM(externalbook.xlsx!TestTable1[[#Totals],['[Column3]:[']Column4]])";
                //CELLSNET-47872
                cells[6, 1].Formula = "VLOOKUP(\"Total\",TestTable1[[#Data],[#Totals]],5,FALSE)";
                Assert.AreEqual("=VLOOKUP(\"Total\",TestTable1[[#Data],[#Totals]],5,FALSE)", cells[6, 1].Formula);
                cells[6, 2].Formula = "VLOOKUP(\"#Column1\",TestTable1[[#Headers],[#Data]],2,FALSE)";
                Assert.AreEqual("=VLOOKUP(\"#Column1\",TestTable1[[#Headers],[#Data]],2,FALSE)", cells[6, 2].Formula);
            }
            if (saveFft != initFft)
            {
                Util.SaveManCheck(wb, "Formula", "Parser_"
                    + Util.GetFileExt(initFft) + "." + Util.GetFileExt(saveFft));
            }
            else
            {
                Util.SaveManCheck(wb, "Formula", "Parser." + Util.GetFileExt(saveFft));
            }
        }
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


