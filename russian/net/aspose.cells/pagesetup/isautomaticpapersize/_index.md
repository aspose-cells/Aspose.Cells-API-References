---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, является ли размер бумаги автоматическим"
type: docs
url: /ru/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Указывает, является ли размер бумаги автоматическим.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к настройкам страницы
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Получить значение автоматического размера бумаги
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // Создайте другую книгу с другими настройками
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


