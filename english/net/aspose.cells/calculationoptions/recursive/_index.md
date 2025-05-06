---
title: CalculationOptions.Recursive
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

```csharp
public bool Recursive { get; set; }
```

### Examples

```csharp
// Called: opts.Recursive = true;
[Test]
        public void Property_Recursive()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET48545.xlsx&quot;);
            int activeIndex = wb.Worksheets.ActiveSheetIndex;

            CalculationOptions opts = new CalculationOptions();
            opts.Recursive = true;
            opts.IgnoreError = false;
            wb.CalculateFormula(opts);
            Worksheet sheet = wb.Worksheets[activeIndex];
            sheet.CalculateFormula(opts, true);

            sheet.Shapes.UpdateSelectedValue();
            wb.Save(Constants.destPath + &quot;CELLSNET48545.xlsx&quot;);
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


