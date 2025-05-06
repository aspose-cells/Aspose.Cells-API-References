---
title: AutoFitterOptions.FormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the formatted strategy
type: docs
url: /net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Gets and sets the formatted strategy.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Remarks

The default value is CellStyle for performance.

### Examples

```csharp
// Called: options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
[Test]
        public void Property_FormatStrategy()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET48473_1.xlsx&quot;);
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            workbook.Worksheets[1].AutoFitColumns(options);
            Cells cells = workbook.Worksheets[1].Cells;
            int w = cells.GetColumnWidthPixel(14 + 0);
            Assert.IsTrue(w == 27 || w == 29);

            w = cells.GetColumnWidthPixel(14 + 1);
            Assert.IsTrue(w == 27 || w == 29);
            w = cells.GetColumnWidthPixel(14 + 2);
            Assert.IsTrue(w == 27 || w == 24);
            workbook.Save(Constants.destPath + &quot;CELLSNET48473_1.xlsx&quot;);

        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


