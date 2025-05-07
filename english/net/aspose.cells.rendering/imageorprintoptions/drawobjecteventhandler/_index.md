---
title: ImageOrPrintOptions.DrawObjectEventHandler
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Implements this interface to get DrawObject and Bound when rendering
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implements this interface to get DrawObject and Bound when rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Examples

```csharp
// Called: imgOrPrintOptions.DrawObjectEventHandler = drawHandler;
[Test]
        public void Property_DrawObjectEventHandler()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-42520.xlsx");
            Worksheet sheet = wb.Worksheets["Sheet1"];

            // Circumvents bug CELLSJAVA-42496
            sheet.AutoFitRows(true);

            // DrawObjectEventHandler
            MyDrawObjectEventHandler drawHandler = new MyDrawObjectEventHandler();

            ImageOrPrintOptions imgOrPrintOptions = new ImageOrPrintOptions();
#if !NETCOREAPP2_0
            imgOrPrintOptions.ImageType = ImageType.Png;
#endif
            imgOrPrintOptions.DrawObjectEventHandler = drawHandler;

            SheetRender render = new SheetRender(sheet, imgOrPrintOptions);

            // trigger the DrawObjectEventHandler by rendering each page
            for (int pg = 0, pages = render.PageCount; pg < pages; pg++)
            {
                drawHandler.PageIndex = pg;
                render.ToImage(pg, new MemoryStream());
            }
        }
```

### See Also

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


