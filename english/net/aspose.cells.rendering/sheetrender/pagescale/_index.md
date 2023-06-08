---
title: SheetRender.PageScale
second_title: Aspose.Cells for .NET API Reference
description: SheetRender property. Gets calculated page scale of the sheet. Returns the set scale if Zoom is set. Otherwise returns the calculated scale according to FitToPagesWide and FitToPagesTall
type: docs
url: /net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Gets calculated page scale of the sheet. Returns the set scale if [`Zoom`](../../../aspose.cells/pagesetup/zoom/) is set. Otherwise, returns the calculated scale according to [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) and [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Examples

```csharp
Workbook wb = new Workbook("Book1.xlsx");

SheetRender sheetRender = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());

//Gets calculated page scale of the sheet.
double pageScale = sheetRender.PageScale;
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


