---
title: "ImageOrPrintOptions.OnePagePerSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться."
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

Если параметр OnePagePerSheet установлен в true, всё содержимое одного листа будет выводиться на одну страницу в результате. Формат бумаги из настройки pagesetup будет недействительным, а остальные настройки pagesetup сохранят своё действие.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
            }

            // Создать параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true; // Key property being demonstrated
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Создайте SheetRender
            SheetRender sr = new SheetRender(worksheet, options);
            
            // Сохраните выходное изображение
            sr.ToImage(0, "OnePagePerSheetOutput.png");
            
            Console.WriteLine("Output saved with OnePagePerSheet=true");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


