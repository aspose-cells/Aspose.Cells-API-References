---
title: SheetRender.PageCount
second_title: Aspose.Cells for .NET API Reference
description: SheetRender property. Gets the total page count of current worksheet
type: docs
url: /net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Gets the total page count of current worksheet.

```csharp
public int PageCount { get; }
```

### Examples

```csharp
// Called: for (int i = 0; i < sheetRender.PageCount; i++)
public void SheetRender_Property_PageCount()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");

    ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
    imgOpt.ImageType = ImageType.Png;
    SheetRender sheetRender = new SheetRender(wb.Worksheets[0], imgOpt);

    for (int i = 0; i < sheetRender.PageCount; i++)
    {
        sheetRender.ToImage(i, new MemoryStream());
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


