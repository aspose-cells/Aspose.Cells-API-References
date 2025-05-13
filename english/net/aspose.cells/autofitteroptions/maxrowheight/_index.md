---
title: AutoFitterOptions.MaxRowHeight
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the max row heightin unit of Point when autofitting rows
type: docs
url: /net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Gets and sets the max row height(in unit of Point) when autofitting rows.

```csharp
public double MaxRowHeight { get; set; }
```

### Examples

```csharp
// Called: MaxRowHeight = int.MaxValue,
public void AutoFitterOptions_Property_MaxRowHeight()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFitColumns(new AutoFitterOptions
    {
        AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
        AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
        MaxRowHeight = int.MaxValue,
        OnlyAuto = true
    });
    //Assert.AreEqual(116, worksheet.Cells.GetColumnWidthPixel(1));

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


