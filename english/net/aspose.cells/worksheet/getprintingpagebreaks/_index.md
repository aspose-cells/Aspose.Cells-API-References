---
title: Worksheet.GetPrintingPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Gets automatic page breaks
type: docs
url: /net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Gets automatic page breaks.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The print options |

### Return Value

The automatic page breaks areas.

### Remarks

Each cell area represents a paper.

### Examples

```csharp
// Called: cellAreas = wb.Worksheets[0].GetPrintingPageBreaks(new ImageOrPrintOptions());
public void Worksheet_Method_GetPrintingPageBreaks() 
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    CellArea[] cellAreas = wb.Worksheets[0].GetPrintingPageBreaks(new ImageOrPrintOptions());

    Assert.AreEqual(44, cellAreas[0].EndRow);

    wb = new Workbook(Constants.sourcePath + "example.xlsx");

    cellAreas = wb.Worksheets[0].GetPrintingPageBreaks(new ImageOrPrintOptions());

    Assert.AreEqual(44, cellAreas[0].EndRow);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


