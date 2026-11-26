---
title: "PageSetup.PrinterSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Получает и задает настройки принтера по умолчанию"
type: docs
url: /ru/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Получает и задает параметры принтера по умолчанию.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Доступ к настройкам страницы
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установить настройки принтера (в виде массива байтов)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Проверьте, что настройки принтера установлены
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Сохраните книгу
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


