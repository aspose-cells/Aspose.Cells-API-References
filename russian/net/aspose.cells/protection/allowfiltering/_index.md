---
title: "Protection.AllowFiltering"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Описывает, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа"
type: docs
url: /ru/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Представляет, разрешено ли пользователю использовать автофильтр, созданный до защиты листа.

```csharp
public bool AllowFiltering { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Включить защиту листа
            worksheet.Protect(ProtectionType.All);
            
            // Установите свойство AllowFiltering в значение true
            worksheet.Protection.AllowFiltering = true;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверьте, что свойство было сохранено корректно
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


