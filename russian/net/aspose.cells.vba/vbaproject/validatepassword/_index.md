---
title: "VbaProject.ValidatePassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProject. Проверяет пароль защиты"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Проверяет пароль защиты.

```csharp
public bool ValidatePassword(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | пароль |

### Возвращаемое значение

Является ли пароль паролем защиты этого проекта VBA

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Создать объект книги из образца файла Excel с проектом VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Проверить пароль проекта VBA
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Вывести результат проверки
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


