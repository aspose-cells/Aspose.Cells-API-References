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
// Called: CellArea[] cellAreas = wb.Worksheets[0].GetPrintingPageBreaks(new ImageOrPrintOptions());
[Test]
        public void Method_ImageOrPrintOptions_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-49873.xlsx&quot;);

            CellArea[] cellAreas = wb.Worksheets[0].GetPrintingPageBreaks(new ImageOrPrintOptions());

            Assert.AreEqual(55, cellAreas[0].EndRow);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


