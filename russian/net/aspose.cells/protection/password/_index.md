---
title: "Protection.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Содержит пароль для защиты листа"
type: docs
url: /ru/net/aspose.cells/protection/password/
---
## Protection.Password property

Представляет пароль для защиты листа.

```csharp
public string Password { get; set; }
```

### Примечания

Если пароль установлен как null или пустая строка, вы можете снять защиту листа или книги без использования пароля. В противном случае необходимо указать пароль для снятия защиты листа или книги.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить настройки защиты с паролем
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Проверьте защиту паролем
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Создайте другой объект защиты для сравнения
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Сравните защиту паролем
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


