---
title: "ImageOrPrintOptions.SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает листы для рендеринга. По умолчанию — все видимые листы в книге Visible"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Возвращает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Примечания

Набор игнорируется, когда используется в [`SheetRender`](../../sheetrender/)

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "VisibleSheet1";
            sheet1.Cells["A1"].PutValue("Sheet1 Content");
            
            Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Content");
            
            Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
            sheet3.Cells["A1"].PutValue("Hidden Content");
            sheet3.IsVisible = false;

            // Продемонстрировать свойство SheetSet с ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;

            // Вариант 1: Печать всех листов (включая скрытые)
            options.SheetSet = SheetSet.All;
            WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");

            // Вариант 2: Печать только видимых листов
            options.SheetSet = SheetSet.Visible;
            WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");

            // Вариант 3: Печать конкретных листов по индексу
            options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
            WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");

            // Сохранить одну страницу в поток в качестве демонстрации
            using (MemoryStream stream = new MemoryStream())
            {
                specificSheetsRender.ToImage(0, stream);
                Console.WriteLine($"Image stream length: {stream.Length} bytes");
            }
        }
    }
}
```

### См. также

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


