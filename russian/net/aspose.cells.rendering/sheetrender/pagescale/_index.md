---
title: "SheetRender.PageScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetRender. Возвращает вычисленный масштаб страницы листа. Возвращает установленный масштаб, если задан Zoom. В противном случае возвращает вычисленный масштаб в соответствии с FitToPagesWide и FitToPagesTall"
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Получает вычисленный масштаб страницы листа. Возвращает установленный масштаб, если [`Zoom`](../../../aspose.cells/pagesetup/zoom/) задан. В противном случае возвращает вычисленный масштаб в соответствии с [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) и [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Создать параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Создайте SheetRender
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Получите и отобразите вычисленный масштаб страницы
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


