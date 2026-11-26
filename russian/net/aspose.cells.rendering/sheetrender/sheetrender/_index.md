---
title: "SheetRender.SheetRender"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SheetRender. Конструктор SheetRender требует worksheet и ImageOrPrintOptions в качестве параметров"
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

конструктор SheetRender, требуется лист и ImageOrPrintOptions в качестве параметров

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| worksheet | Worksheet | Укажите, какую таблицу необходимо отобразить. |
| опции | ImageOrPrintOptions | ImageOrPrintOptions содержит некоторые свойства выходного изображения |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу и добавьте некоторые примерные данные.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Создайте SheetRender с Worksheet и ImageOrPrintOptions.
            SheetRender render = new SheetRender(worksheet, options);

            // Вывести количество страниц
            Console.WriteLine("Page count: " + render.PageCount);

            // Сохраните отрисованное изображение.
            render.ToImage(0, "output.png");
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


