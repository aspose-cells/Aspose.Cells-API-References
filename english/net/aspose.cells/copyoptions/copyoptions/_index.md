---
title: CopyOptions.CopyOptions
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions constructor. CopyOptions constructor
type: docs
url: /net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions constructor.

```csharp
public CopyOptions()
```

### Examples

```csharp
// Called: CopyOptions copyOptions = new CopyOptions { CopyInvalidFormulasAsValues = true };
[Test]
        public void CopyOptions_Constructor()
        {
            var modelWorkbook = new Workbook(Constants.sourcePath + &quot;CellsNet55001.xlsx&quot;);

            // Originally, we populate transactional data here - but the test works without.

            modelWorkbook.CalculateFormula();

            // For 21.12 versions:
            // modelWorkbook.Settings.CreateCalcChain = false;
            // For later versions:
            modelWorkbook.Settings.FormulaSettings.EnableCalculationChain = false;
            Workbook subWorkbook = new Workbook();

            CopyOptions copyOptions = new CopyOptions { CopyInvalidFormulasAsValues = true };
            Worksheet justAddedSheet = subWorkbook.Worksheets.Add(&quot;Industry Summary&quot;);

            justAddedSheet.Copy(modelWorkbook.Worksheets[&quot;Industry Summary&quot;], copyOptions);
            Util.ReSave(subWorkbook, SaveFormat.Xlsx);
            //subWorkbook.Save(Constants.destPath + &quot;CellsNet55001.xlsx&quot;);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


