---
title: Cells.Clear
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears all data of the worksheet
type: docs
url: /net/aspose.cells/cells/clear/
---
## Cells.Clear method

Clears all data of the worksheet.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: cells.Clear();
public void Cells_Method_Clear()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.Formula = "=Cells_Method_Clear(3)";
    cell.Calculate(new CalculationOptions());
    double v = cell.DoubleValue;
    if (v < 0.0 || v > 1.0)
    {
        Assert.Fail("Value of " + cell.Formula + " is out of range: " + v);
    }

    cell.Formula = "=Cells_Method_Clear(3,1,-0.2,-0.1)";
    cell.Calculate(new CalculationOptions());
    v = cell.DoubleValue;
    if (v < -0.2 || v > -0.1)
    {
        Assert.Fail("Value of " + cell.Formula + " is out of range: " + v);
    }

    cell.Formula = "=Cells_Method_Clear(3,1,0.1,0.2,0.1)";
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual("#VALUE!", cell.StringValue, "Value of " + cell.Formula);

    cell.SetDynamicArrayFormula("=Cells_Method_Clear(3,2,-0.2,-0.1)", new FormulaParseOptions(), true);
    int sameCount = 0;
    double prev = -1;
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 2; j++)
        {
            Cell c = cells.CheckCell(i, j);
            if (c == null || !c.IsFormula)
            {
                Assert.Fail(CellsHelper.CellIndexToName(i, j) + " should be spilled as formula but was not");
            }
            v = c.DoubleValue;
            if (v < -0.2 || v > -0.1)
            {
                Assert.Fail("Value of " + c.Name + c.Formula + " is out of range: " + v);
            }
            if (v == prev)
            {
                sameCount++;
            }
            else
            {
                prev = v;
            }
        }
    }
    if (sameCount > 0)
    {
        Assert.Fail("This message should not be poped up frequently."
            + " Rare situation arises:\nDifferent cells with RAND formula should give different values, same count is "
            + sameCount);
    }

    cells.Clear();
    cell = cells[0, 0];
    cell.SetDynamicArrayFormula("=Cells_Method_Clear(3,2,-0.1,-0.1)", new FormulaParseOptions(), true);
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 2; j++)
        {
            Cell c = cells.CheckCell(i, j);
            if (c == null || !c.IsFormula)
            {
                Assert.Fail(CellsHelper.CellIndexToName(i, j) + " should be spilled as formula but was not");
            }
            v = c.DoubleValue;
            if (v != -0.1)
            {
                Assert.Fail("Value of " + c.Name + c.Formula + " is out of range: " + v);
            }
        }
    }

    cells.Clear();
    cell = cells[0, 0];
    cell.SetDynamicArrayFormula("=Cells_Method_Clear(30,20,2,3,0.1)", new FormulaParseOptions(), true);
    bool no2 = true;
    bool no3 = true;
    for (int i = 0; i < 30; i++)
    {
        for (int j = 0; j < 20; j++)
        {
            Cell c = cells.CheckCell(i, j);
            if (c == null || !c.IsFormula)
            {
                Assert.Fail(CellsHelper.CellIndexToName(i, j) + " should be spilled as formula but was not");
            }
            v = c.DoubleValue;
            if (v == 2.0)
            {
                no2 = false;
            }
            else if (v == 3.0)
            {
                no3 = false;
            }
            else
            {
                Assert.Fail("Value of " + c.Name + c.Formula + " is out of range: " + v);
            }
        }
    }
    if (no2)
    {
        Assert.Fail("No value 2 in the results");
    }
    if (no3)
    {
        Assert.Fail("No value 3 in the results");
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


