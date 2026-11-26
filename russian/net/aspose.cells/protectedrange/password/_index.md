---
title: "ProtectedRange.Password"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ProtectedRange. Представляет пароль для защиты диапазона"
type: docs
url: /ru/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Представляет пароль для защиты диапазона.

```csharp
public string Password { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию защищённых диапазонов
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Добавить защищённый диапазон
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Установить пароль для защищённого диапазона
            protectedRange.Password = "12345";

            // Сохраните книгу
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### См. также

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


