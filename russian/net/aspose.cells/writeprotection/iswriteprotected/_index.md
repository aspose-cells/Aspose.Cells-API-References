---
title: "WriteProtection.IsWriteProtected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WriteProtection property. Указывает, защищена ли эта рабочая книга от записи"
type: docs
url: /ru/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Указывает, защищена ли эта рабочая книга от записи.

```csharp
public bool IsWriteProtected { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Включите защиту от записи с паролем
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Проверьте, защищена ли рабочая книга от записи
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Проверить пароль
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Сохраните книгу
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Загрузите сохранённую рабочую книгу, чтобы проверить защиту
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Снова проверьте статус защиты
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### См. также

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


