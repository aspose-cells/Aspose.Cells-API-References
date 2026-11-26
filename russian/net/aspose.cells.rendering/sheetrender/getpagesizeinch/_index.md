---
title: "SheetRender.GetPageSizeInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SheetRender. Получить размер страницы в дюймах выходного изображения."
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Получить размер страницы в дюймах выходного изображения.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы начинается с нуля. |

### Возвращаемое значение

Размер изображения, [0] — ширина и [1] — высота

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


