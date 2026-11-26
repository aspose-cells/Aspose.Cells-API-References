---
title: "Protection.VerifyPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Protection. Проверяет пароль"
type: docs
url: /ru/net/aspose.cells/protection/verifypassword/
---
## Protection.VerifyPassword method

Проверяет пароль.

```csharp
public bool VerifyPassword(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | Пароль. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodVerifyPasswordWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Защитить лист паролем
            worksheet.Protection.AllowDeletingColumn = false;
            worksheet.Protection.AllowDeletingRow = false;
            worksheet.Protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Проверить пароль
                bool isPasswordCorrect = worksheet.Protection.VerifyPassword("password123");
                
                Console.WriteLine($"Password verification result: {isPasswordCorrect}");
                
                if (isPasswordCorrect)
                {
                    Console.WriteLine("The provided password matches the worksheet protection password.");
                }
                else
                {
                    Console.WriteLine("The provided password does not match the worksheet protection password.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing VerifyPassword method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


