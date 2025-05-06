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
// Called: modelWorkbook.Settings.FormulaSettings.EnableCalculationChain = false;
[Test]
        public void Property_FormulaSettings()
        {
            var modelWorkbook = new Workbook(Constants.sourcePath + &quot;CELLSNET54992.xlsx&quot;);

            // Originally, we populate transactional data here - but the test works without.

            modelWorkbook.CalculateFormula();

            // For 21.12 versions:
            // modelWorkbook.Settings.CreateCalcChain = false;
            // For later versions:
            modelWorkbook.Settings.FormulaSettings.EnableCalculationChain = false;
            Workbook subWorkbook = new Workbook();

            CopyOptions copyOptions = new CopyOptions { CopyInvalidFormulasAsValues = true };
            Worksheet justAddedSheet = subWorkbook.Worksheets.Add(&quot;TM_TableOutput&quot;);

            justAddedSheet.Copy(modelWorkbook.Worksheets[&quot;TM_TableOutput&quot;], copyOptions);
            Util.ReSave(subWorkbook, SaveFormat.Xlsx);
            //subWorkbook.Save(Constants.destPath + &quot;CELLSNET54992.xlsx&quot;);
        }
```

### See Also

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


