---
title: Cells.GetRowHeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the height of a specified row in unit of pixel
type: docs
url: /net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Gets the height of a specified row in unit of pixel.

```csharp
public int GetRowHeightPixel(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |

### Return Value

Height of row

### Examples

```csharp
// Called: Assert.AreEqual(18, _worksheet.Cells.GetRowHeightPixel(13));
public void Cells_Method_GetRowHeightPixel()
{
    // Instantiate a new Workbook
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    // Get the first (default) worksheet
    Worksheet _worksheet = wb.Worksheets[0];

    // Create an object for AutoFitterOptions
    AutoFitterOptions options = new AutoFitterOptions();

    // Set auto-fit for merged cells
    options.AutoFitMergedCells = (true);

    // Autofit rows in the sheet(including the merged cells)
    _worksheet.AutoFitRows(options);
    Assert.AreEqual(18, _worksheet.Cells.GetRowHeightPixel(13));
    Assert.AreEqual(45,_worksheet.Cells.GetRowHeightPixel(18));
    // Save the Excel file
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


