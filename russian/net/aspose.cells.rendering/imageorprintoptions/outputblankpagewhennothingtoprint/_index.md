---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Указывает, следует ли выводить пустую страницу, когда нечего печатать"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Указывает, следует ли выводить пустую страницу, когда нечего печатать.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Примечания

По умолчанию false.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Создать новую пустую рабочую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу, который пуст
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Продемонстрировать свойство OutputBlankPageWhenNothingToPrint
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Отобразить лист
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Вывод всё равно будет содержать одну пустую страницу из‑за настройки свойства
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Сохранить первую страницу в поток памяти
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Теперь установите свойство в false
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // Вывод теперь будет содержать ноль страниц
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


