---
title: "PageSetup.PaperHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Возвращает высоту бумаги в дюймах, учитывая ориентацию страницы"
type: docs
url: /ru/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Получает высоту бумаги в дюймах, учитывая ориентацию страницы.

```csharp
public double PaperHeight { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить некоторые данные в ячейку
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Получить объект PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Отобразить высоту бумаги по умолчанию (в дюймах)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight доступен только для чтения, поэтому мы демонстрируем получение разных размеров бумаги
            // изменив тип размера бумаги на Letter (8,5×11 дюймов)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Проверьте изменение
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


