---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает булево значение, которое определяет, автоматически сжимает ли приложение изображения в книге"
type: docs
url: /ru/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Указывает логическое значение, которое определяет, автоматически сжимает ли приложение изображения в рабочей книге.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Включить AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Добавьте пример изображения для демонстрации сжатия
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить настройку
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


