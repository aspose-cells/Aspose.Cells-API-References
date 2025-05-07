---
title: WorkbookSettings.FormulaSettings
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the settings for formularelated features
type: docs
url: /net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Gets the settings for formula-related features.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Examples

```csharp
// Called: wb.Settings.FormulaSettings.EnableCalculationChain = true;
[Test]
        public void Property_FormulaSettings()
        {
            Workbook wb = new Workbook();
            Cells cellsF = wb.Worksheets[0].Cells;
            Name name = wb.Worksheets.Names[wb.Worksheets.Names.Add("TESTNAME")];
            name.RefersTo = "Sheet1!$A$2:$B$3";
            cellsF["A1"].Formula = "=SUM(TESTNAME)";
            cellsF["A2"].PutValue(1);
            cellsF["B2"].PutValue(2);
            cellsF["A3"].PutValue(4);
            cellsF["B3"].PutValue(8);
            wb.Settings.FormulaSettings.EnableCalculationChain = true;
            wb.CalculateFormula();
            Assert.AreEqual(15, cellsF["A1"].IntValue, "First calc");
            string[] expectedA1 = new string[] { "Sheet1!A1", };
            CheckDependentsInCalculation("Leaf1-", cellsF["A2"], false, expectedA1);
            CheckDependentsInCalculation("Leaf1-", cellsF["A3"], false, expectedA1);
            CheckDependentsInCalculation("Leaf1-", cellsF["B2"], false, expectedA1);
            CheckDependentsInCalculation("Leaf1-", cellsF["B3"], false, expectedA1);
            CalculationOptions copt = new CalculationOptions();
            name.RefersTo = "Sheet1!$B$2:$B$3";
            wb.CalculateFormula();
            Assert.AreEqual(10, cellsF["A1"].IntValue, "Second calc");
            CheckDependentsInCalculation("Leaf1-", cellsF["A2"], false, null);
            CheckDependentsInCalculation("Leaf1-", cellsF["A3"], false, null);
            CheckDependentsInCalculation("Leaf1-", cellsF["B2"], false, expectedA1);
            CheckDependentsInCalculation("Leaf1-", cellsF["B3"], false, expectedA1);
        }
```

### See Also

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


