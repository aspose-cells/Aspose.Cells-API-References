---
title: "Worksheet.CodeName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает кодовое имя листа"
type: docs
url: /ru/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Получает кодовое имя рабочего листа.

```csharp
public string CodeName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Отобразить кодовое имя по умолчанию
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Изменить кодовое имя
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Добавить новый лист и показать его кодовое имя
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Сохраните книгу
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


