---
title: PageSetup.CustomPaperSize
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets the custom paper size in unit of inches
type: docs
url: /net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Sets the custom paper size, in unit of inches.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| width | Double | The width of the paper. |
| height | Double | The height of the paper. |

### Examples

```csharp
// Called: workbook.Worksheets[0].PageSetup.CustomPaperSize(1.5,1.5);
public void PageSetup_Method_CustomPaperSize()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].PageSetup.CustomPaperSize(1.5,1.5);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


