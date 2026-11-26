---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Если PrintWithStatusDialog  true  будет отображаться диалог, показывающий текущий статус печати. иначе такой диалог не будет показан"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати. В противном случае такой диалог не будет показан.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Инициализировать рабочую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Установить параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Создайте SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // Печать в PDF
            sheetRender.ToImage(0, "output.png");

            // Ожидать создания файла (упрощённая логика ожидания)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


