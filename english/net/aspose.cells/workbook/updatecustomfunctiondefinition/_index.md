---
title: Workbook.UpdateCustomFunctionDefinition
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Updates definition of custom functions
type: docs
url: /net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Updates definition of custom functions.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |

### Remarks

This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

### Examples

```csharp
// Called: wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());
public void Workbook_Method_UpdateCustomFunctionDefinition()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[0, 1].PutValue(1);
    cells[0, 2].PutValue(2);
    cells[1, 1].PutValue(4);
    cells[1, 2].PutValue(8);
    ArrayModeParamEngine ce = new ArrayModeParamEngine();
    CalculationOptions copts = new CalculationOptions();
    copts.CustomEngine = ce;
    FormulaCaseUtil.AssertInt(3, sheet.CalculateFormula("=MYFUNC(B:B+C:C)", copts), "ValueMode");
    ce._arrayMode = true;
    FormulaCaseUtil.AssertInt(15, sheet.CalculateFormula("=MYFUNC(B:B+C:C)", copts), "ArrayMode");

    FormulaParseOptions popts = new FormulaParseOptions();
    popts.CustomFunctionDefinition = new MyCustomFunctionDefinition();
    ce._arrayMode = false;
    ce._autoMode = true;
    FormulaCaseUtil.AssertInt(48, sheet.CalculateFormula("=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)",
        popts, copts, 0, 0, null), "Parsed ArrayMode");

    Cell cell = cells[0, 0];
    cell.Formula = "=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)";
    wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());
    wb.CalculateFormula(copts);
    FormulaCaseUtil.AssertInt(48, cell.Value, "Updated ArrayMode");
}
```

### See Also

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


