---
title: FormulaSettings.EnableCalculationChain
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Whether enable calculation chain for formulas. Default is false
type: docs
url: /net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Whether enable calculation chain for formulas. Default is false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Remarks

When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### Examples

```csharp
// Called: modelWorkbook.Settings.FormulaSettings.EnableCalculationChain = false;
public void FormulaSettings_Property_EnableCalculationChain()
{
    var modelWorkbook = new Workbook(Constants.sourcePath + "example.xlsx");

    // Originally, we populate transactional data here - but the test works without.

    modelWorkbook.CalculateFormula();

    // For 21.12 versions:
    // modelWorkbook.Settings.CreateCalcChain = false;
    // For later versions:
    modelWorkbook.Settings.FormulaSettings.EnableCalculationChain = false;
    Workbook subWorkbook = new Workbook();

    CopyOptions copyOptions = new CopyOptions { CopyInvalidFormulasAsValues = true };
    Worksheet justAddedSheet = subWorkbook.Worksheets.Add("Industry Summary");

    justAddedSheet.Copy(modelWorkbook.Worksheets["Industry Summary"], copyOptions);
    Util.ReSave(subWorkbook, SaveFormat.Xlsx);
    //subWorkbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


