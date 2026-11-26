---
title: "PageSetup.PaperWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Возвращает ширину листа в дюймах с учётом ориентации страницы"
type: docs
url: /ru/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Получает ширину бумаги в дюймах, учитывая ориентацию страницы.

```csharp
public double PaperWidth { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Получить доступ к PageSetup листа
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Продемонстрировать свойство PaperWidth (только для чтения)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Чтобы изменить размер листа, используйте свойство PaperSize
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


