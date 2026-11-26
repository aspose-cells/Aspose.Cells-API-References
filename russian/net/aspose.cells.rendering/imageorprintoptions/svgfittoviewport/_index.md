---
title: "ImageOrPrintOptions.SVGFitToViewPort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Если это свойство истинно, сгенерированный svg будет соответствовать области просмотра"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

Если это свойство равно true, сгенерированный SVG будет подгоняться под область просмотра.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте [`FitToViewPort`](../../svgimageoptions/fittoviewport/). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySVGFitToViewPortDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Создать параметры изображения для вывода SVG
            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true; // This is the key property being demonstrated
            
            // Отрисовать лист в SVG‑изображение
            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, "output.svg");
            
            Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


