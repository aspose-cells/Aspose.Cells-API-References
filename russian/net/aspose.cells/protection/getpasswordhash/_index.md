---
title: "Protection.GetPasswordHash"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Protection. Получает хеш текущего пароля"
type: docs
url: /ru/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Получает хеш текущего пароля.

```csharp
public int GetPasswordHash()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить настройки защиты с паролем
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Защитить лист
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Получить хеш пароля
                int passwordHash = protection.GetPasswordHash();
                
                // Отобразить результат
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Проверить пароль (демонстрация связанной функциональности)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


