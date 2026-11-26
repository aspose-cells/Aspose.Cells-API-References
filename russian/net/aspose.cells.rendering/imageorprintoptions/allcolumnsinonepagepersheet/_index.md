---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках страницы будет недействительна, а остальные настройки pagesetup по‑прежнему будут применяться."
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках страницы будет недействительной, а остальные настройки pagesetup по‑прежнему будут применяться.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторые данные в листе
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Создать параметры сохранения изображения
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // Сохранить книгу в поток памяти в формате PNG
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


