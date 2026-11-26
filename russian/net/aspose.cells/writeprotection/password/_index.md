---
title: "WriteProtection.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WriteProtection property. Устанавливает защищённый пароль для изменения файла"
type: docs
url: /ru/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Устанавливает защищённый пароль для изменения файла.

```csharp
public string Password { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пароль защиты от записи
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Сохраните книгу
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### См. также

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


