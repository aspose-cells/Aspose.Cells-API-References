---
title: CopyOptions.CopyInvalidFormulasAsValues
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. If the formula is not valid for the dest destination only copy values
type: docs
url: /net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

If the formula is not valid for the dest destination, only copy values.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Examples

```csharp
// Called: CopyOptions copyOptions = new CopyOptions { CopyInvalidFormulasAsValues = true };
[Test]
        public void Property_CopyInvalidFormulasAsValues()
        {
            var modelWorkbook = new Workbook(Constants.sourcePath + "CellsNet55001.xlsx");

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
            //subWorkbook.Save(Constants.destPath + "CellsNet55001.xlsx");
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


