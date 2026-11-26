---
title: "WriteProtection.ValidatePassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WriteProtection method. Возвращает true, если указанный пароль совпадает с паролем защиты от записи, которым файл был защищён"
type: docs
url: /ru/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Возвращает true, если указанный пароль совпадает с паролем защиты от записи, которым файл был защищён.

```csharp
public bool ValidatePassword(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | Указанный пароль. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите пароль защиты от записи
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Проверьте пароль
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### См. также

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


