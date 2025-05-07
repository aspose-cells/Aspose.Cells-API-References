---
title: AutoFitterOptions.AutoFitMergedCells
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Indicates whether auto fit row height when the cells is merged in a row. The default value is false
type: docs
url: /net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Indicates whether auto fit row height when the cells is merged in a row. The default value is false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: options.AutoFitMergedCells = (true);
[Test]
       public void Property_AutoFitMergedCells()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET46605_1.xlsx");

            AutoFitterOptions options = new AutoFitterOptions();

            // Set auto-fit for merged cells
            options.AutoFitMergedCells = (true);

            // Autofit rows in the sheet(including the merged cells)
            wb.Worksheets[0].AutoFitRows(options);
            Assert.AreEqual(20, wb.Worksheets[0].Cells.GetRowHeightPixel(11));

            wb.Save(Constants.destPath + "CELLSNET46605_1.xlsx");

            wb = new Workbook(Constants.sourcePath + "CELLSNET46605_2.xlsx");

            options = new AutoFitterOptions();

            // Set auto-fit for merged cells
            options.AutoFitMergedCells = (true);

            // Autofit rows in the sheet(including the merged cells)
            wb.Worksheets[0].AutoFitRows(options);
            Assert.AreEqual(20, wb.Worksheets[0].Cells.GetRowHeightPixel(11));

            wb.Save(Constants.destPath + "CELLSNET46605_1.xlsx");
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


