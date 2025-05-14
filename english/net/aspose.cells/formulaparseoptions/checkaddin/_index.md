---
title: FormulaParseOptions.CheckAddIn
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Whether check addins in existing external links of current workbook for user defined function without external link. Default is trueif user defined function matches one addin in existing external links then take it as the addin
type: docs
url: /net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

```csharp
public bool CheckAddIn { get; set; }
```

### Examples

```csharp
// Called: cells[0, c1++].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false }, null);
public void FormulaParseOptions_Property_CheckAddIn()
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

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


