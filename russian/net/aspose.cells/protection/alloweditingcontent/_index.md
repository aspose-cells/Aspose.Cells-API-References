---
title: "Protection.AllowEditingContent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе.

```csharp
public bool AllowEditingContent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Защитить лист паролем
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Проверить и отобразить свойство AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Изменить свойство AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // Проверить и отобразить обновлённое свойство
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Сохраните книгу
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


