---
title: "Protection.IsProtectedWithPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, защищён ли лист паролем"
type: docs
url: /ru/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Указывает, защищён ли лист паролем.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к настройкам защиты листа
            Protection protection = worksheet.Protection;

            // Установите пароль защиты
            protection.Password = "test123";

            // Проверьте, защищён ли лист паролем
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Сохраните книгу
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


